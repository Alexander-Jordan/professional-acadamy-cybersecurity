# Unit 2: Cryptography & Encryption

## Summary

In this unit we covered:

- History of Cryptography
- Encryption & Decryption
- Cryptographic Protocols
- Hash Functions

## U2P1: Unit introduction

Objectives for unit 2:

- Understand cryptographic techniques
- Understand the different encryption algorithms
- Understand the different hashing algorithms
- Overview of different cryptography tools and hash calculators
- Understand Public Key Infrastructure (PKI) and certificate management concepts
- Understand various application of cryptography

A lot will only be gently introduced, but the main part to learn is:

- Understand the difference between symmetric & asymmetric encryption
- Know where to find information about cryptography & encryption

## U2P2-4: Intro to ciphers - What is cryptography?

- **Cryptography:** The art or science concerning the principles, means, and methods for converting plaintext into ciphertext and for restoring encrypted ciphertext to plaintext. The making. Cryptographers.
- **Cryptanalysis:** The operations performed in defeating or circumventing cryptographic protection of information by applying mathematical techniques. The breaking. Cryptanalysts.
- **Cryptology:** The mathematical science that deals with cryptanalysis and cryptography. The art and science of making an breaking "secret codes". Cryptologists.
- **Cipher:** A cryptographic algorithm.
- **Plaintext:** Unencrypted information.
- **Ciphertext:** Data or informatino in its encrypted form.
- **Decipher/Encipher:** To convert enciphered text to plaintext by means of a cryptographic system and vice versa.

### Why use cryptography?

- Secure banking, mobile communications, wireless networks, files.
- Authenticating electronic documents
- Electronic voting
- Digital Rights Management (DRM)
- Crypto currencies

### Goals (PAIN)

- **Privacy:** confidentiality, protect the secrets
- **Authentication:** roving who sent it
- **Integrity:** ensuring integrity via hashing message digests
- **Non-repudiation:** vial digital signature, digital certs and Public Key Infrastructure (PKI)

### Through the ages

- Egyptians: hieroglyphics (at least needed to be decrypted to be understandable by us)
- Spartans: scytale

Up until 1970, we only has symmetric encryption, which include an "unbreakable" secret code, but everything a human can come up with, another human can resolve eventually.

Today cryptography and encryption is still important, and harder to break.
Quantum computers is a threat to that.
Criminals steal encrypted data for later when quantum computing is here.

### What is a cipher?

- Method for encrypting a message
- Encryption algorithms are standardized & published (, , and the most important thing to keep secret is the key (think padlock vs key analogy))
  - they are open for public scrutiny
  - threats are discovered sooner
  - the most important thing to keep secret is the **key**, not the padlock (algorithm)
  - analogy: knowing how a padlock works, doesn't mean you can unlock all padlocks, you still need the key
- The key (cryptovariable): input to the algorithm

> [!NOTE]  
> Symmetric algorithm: the same key is used for encrypting and decrypting.  
> Asymmetric algorithm: different keys are used for encrypting and decrypting.  

### Cryptosystem

The hardware or software implementation that transforms plaintext into cipher text (encrypting) and back into plaintext (decrypting). It's efficient, easy to use, and the strength is based on keys rather than algorithm.

### Substitution cipher (caesar cipher)

A monoalphabetic cypher.

Each letter in the alphabet is rotated by three letters:

- A -> D
- B -> E
- C -> F
- ...

The flaws: it's too simple/easy to crack

### Substitution cipher (monoalphabetic)

Any letter can be substituted for any other letter (unique substitute).

Brute force would be too time consuming.

### Vigenere cipher

A polyalphabetic cipher.

Introduces having a key.

> Encrypting: the cipher letter is found at the intersection of the column headed by the plaintext letter and the row indexed by the key letter.  
> Decrypting: the plaintext letter is found at the head of the column determined by the intersection of the diagonal containing the cipher letter and the row containing the key letter.  

## U2P5: Activity

Encrypt a song title using the Vigenere cipher.

- Song title: Two Little Birds
- Key: BobMarley
- Encrypted title: Ukp Xikepc Cwsps

| Plaintext | Key | Encrypted |
|:---:|:---:|:---:|
| T | B | U |
| W | O | K |
| O | B | P |
| L | M | X |
| I | A | I |
| T | R | K |
| T | L | E |
| L | E | P |
| E | Y | C |
| B | B | C |
| I | O | W |
| R | B | S |
| D | M | P |
| S | A | S |

## U2P6-7: Symmetric encryption

Uses the same key for encryption and decryption.

- Strength is determined by the size of the key.
- Key length is expressed in bits.
- Set of possible keys for a cipher is called key space.
- To crack the key the hacker has to use brute-force.

Pros:

- Fast transfer
- Strong privacy

Cons:

- Out of band key distribution (how to share?)
- Doesn't scale well
- No non-repudiation (integrity/authentication)

Synonyms: Secret, private, shared, session

Classes:

- Stream: one bit at a time
- Block: chunks

### Modern cryptography

DES: Data Encryption Standard (developed by IBM in 1976).  
Being phased out for AES (Advanced Encryption Standard).

- Encipher/Decipher blocks of data consisting of 64-bits under control of a 56-bit key
- Transforms a plaintext to a ciphertext of the same bit length
- Due to inherit weakness of DES, some triple repeats the process (3DES) until they can afford an update to their equipment to AES

### Randomness

Computer are good at some stuff, and bad at some other stuff. One thing they are bad at is random numbers.

<https://www.youtube.com/watch?v=1cUUfMeOijg>

## U2P8-9: AES (Advanced Encryption Standards)

Replacing DES, since 2001.

Not the best, but most used.

Used in:

- Wireless security
- Processor security & file encryption
- SSL/TLS protocol
- WiFi security
- Mobile app encryption
- VPN
- Many government agencies

Attacks:

- 128-bit keys: brute-force is not possible in our current tech
- Side-channel attacks (supporting technologies, like instead of trying to crack the keys, find where the keys are stored)

Symmetric Limitations:

- Only one key to encrypt & decrypt, so the key needs to be transferred to the recipient
- Potential for eavesdropping attacks
- Key Distribution Problem

## U2P10-11: Asymmetric Encryption

Uses a key-pair (public (for encryption) and private (for decryption) key)

- A user generates a key-pair (a public and private key)
- The public key is shared to anyone the owner of the key-pair wants to receive messages from
- The public key is used to encrypt plaintext to be sent to the owner of the key-pair
- The private key is used to decrypt cyphertext by the owner of the key-pair

The key to decrypt messages stays private, and the key to encrypt messages can be freely shared.

This means that a bad actor can't decrypt any cyphertext even if they have access to the public key.

Most popular algorithms:

- RSA (Rivest Shamir Adleman)
- El Gamal
- Ed25519 [RSA vs Ed25519](https://www.geeksforgeeks.org/devops/rsa-vs-ed25519-which-key-pair-is-right-for-your-security-needs/)

Protocols:

- PGP (Pretty Good Privacy)
- S/MIME (Secure/Multipurpose Internet Mail Extension)
- SSL (Secure Socket Layer) & TLS (Transport Layer Socket)

### Hybrid cryptography

What we'd like:

- Privacy
- Authentication
- Integrity
- Non-repudiation
- Speed

Using just symmetric/asymmetric doesn't provide ALL of these.

Hybrid cryptography:

- A random session key is generated by one party (initiator)
- A public key contained in a provided or obtained digital certificate (GAL (Global Address List)) is used to encrypt the one-time session key
- The encrypted symmetric session key is transmitted
- Recipient decrypts the session key with their private key
- An encrypted verification message is sent verifying success
  - Encrypted using the session key and a fast symmetric (AES)
- If the verification is able to be decrypted upon receipt at the session initiator the symmetric key exchange is successful
- Once a session is over the shared key is discarded

Or in simpler terms:

- Sender generates a session key
- Encrypts session key with recipient's public key and sends it
- Recipient decrypts session key
- Both users have same key and switch to faster symmetric AES

Even simpler: asymmetric encryption is used to transfer a symmetric key to be used for all future encryption/decryption.

This ensures a secure transfer of the key, but you utilize the fast speed of symmetric encryption/decryption.

<https://www.youtube.com/watch?v=VPvZbMXfv_0>

## U2P13: Key Agreement

A method to create secret key by exchanging only public keys.

Each party uses the other's public key and their own private key to compute the shared secret key.

Both will end up with the same secret key, by only sharing their public key.

### Summary of symmetric vs. asymmetric

| Attributes | Symmetric | Asymmetric |
|:---:|:---:|:---:|
| Keys | Same key is used by sender to encrypt and receiver to decrypt | Each user has a key pair – a public key and a private key |
| Key Exchange | Out-of-band | Public key is freely shared |
| Speed | Algorithm is less complex and much faster | Algorithm is more complex and slower |
| Number of keys | N*(N-1)/2 | 2N |
| Use | Bulk encryption. Encrypting files and communication. | Key encryption and digital signatures. |
| Security Service Provided | Confidentiality | Confidentiality, authentication and non-repudiation. |

## U2P14-15: Hashing

### Message authentication

Ensures integrity:

- Message hasn't been altered
- Isn't a replay of a previous message
- Sent from the stated origin
- Sent to the intended recipient

### Integrity

How to trust that the file received is the file sent?

- Hashing (MD-5, SHA)
- Integrity checks
- MACs (Message Authentication Code's)

### Hashing Algorithm

- One-way function that converts a data string into a numeric string output of fixed length. Usually smaller.
  - So if a hash is generated from a file, and then the file is altered with only one character, the new hash would be completely new. This is then used for comparison.
- Designed to be collision-resistant
- Same input always gives the same output
- Common hash algorithms are the MD5 (Message-Digest algorithm 5) and the SHA (Secure Hash Algorithm)

### Used

- Integrity checks
- Secure storage of passwords
- Digital Signatures
- Crypto currency
- Generation of pseudorandom bits
- MACs/HMACs

### Integrity check (example: ISB number)

- **ISBN:** 978-0-470-22968-2
- Digit in position 13 (`2`) is a "check" digit calculated by a sum of the
other digits.
- The numbers in positions 1, 3, 5, 7, 9, & 11 are added together
- The numbers in positions 2, 4, 6, 8, 10,  & 12 added together and multiplied with 3
- The first sum is added with the second sum
- Then subtract the last digit of the result from 10
- Answer = 13th digit of ISBN

> `(9+8+4+0+2+6) + 3 * (7+0+7+2+9+8) = 29 + 3 * (33) = 128`  
> `10 – 8 = 2`

### MAC (Message Authentication Code)

- A string of bits that is sent alongside a message
- Depends on the message itself and a secret key (should be able to compute MAC without the key)
- This allows two people who share a secret key to send messages to each other without fear that someone else will tamper with the messages without detection.

The generated MAC can be verified by both parties using the message and secret key, by regenerating a MAC and comparing with the first one. If they are not equal, it is invalid and the message has been altered.

### Hash vs. symmetric vs. asymmetric

- Hash is 1-way (can't decrypt a hash to the original message)
- Symmetric is using 1 key
- Asymmetric is using 2 keys

### Web traffic

- Application (UI): web browser & server
- Protocol (rules of communication): HTTP or HTTPS
- Cryptosystem (framework to provide data protection): SSL or TLS
- Algorithm (encryption math): AES

### Mail

- Application (UI): mail client (outlook) & server (exchange)
- Protocol (rules of communication): Secure SMTP or Secure POP3 pr Secure IMAP
- Cryptosystem (framework to provide data protection): S/MIME or PGP
- Algorithm (encryption math): AES

### HTTP/HTTPS/SSL/TLS

- HTTP (Hypertext Transfer Protocol)
  - Used for viewing web pages
  - All information is sent in clear text
  - Vulnerable to hackers
- HTTPS (Secure Hypertext Transfer Protocol)
  - As HTTP, but with a security feature
  - Encrypts the data
  - Is the default protocol by the majority of websites, regardless if sensitive data is going to be exchanged or not
  - Google is flagging websites as `not secured` if they are not SSL protected
- SSL (Secure Sockets Layer)
  - Ensure security on the internet
  - Uses public key encryption to secure data
  - The server will respond with an SSL certificate when requested to authenticate the identity of a website
- TLS (Transport Layer Security)
  - Latest industry standard & successor to SSL
  - Authenticates server, client, and encrypts data

## U2P16-17: PKI & Activity

### PKI (Public Key Infrastructure)

Ensure secure communication between entities (individuals/websites) online.

- CA (Certificate Authority): issues certificates, maintains and published status information and CRLs (Certificate Revocation Lists) and maintains archives
- RA (Registration Authority): responsible for verifying the certificate contents for the CA
- Repository: accepts certificate and CRLs from a CA and distributes them to authorized parties: OSCP (Online Certificate Status Protocol)
Archive: offers long-term storage of archived information from the CA

### Digital signatures

A way of ensuring integrity & authentication.

- The signer generates a hash of the document (the fingerprint)
- The hash is encrypted using the signers **private** key, forming the digital signature
- The document and the digital signature is sent to the recipient
- The recipient decrypts the digital signature using the signers **public** key
- The recipient generates a hash of the document (the fingerprint), and compares with the hash sent by the recipient
- If they match, the signature is valid, confirming the documents integrity and the signers identity

So in simpler terms: the signer encrypt the hash generated out of the data, using their **private** key, and it's decrypted by the recipient using the signers **public** key.

### Activity

#### Encoding vs encryption

Contrary to encryption, the main purpose is data usability, not confidentiality. The main aim of encoding is to transform data so it can be used by a different type of system.

There is no keys used to encode or decode the data, and knowing how an encoding algorithm works one could decode it easily.

Examples of encoding algorithm: ASCII, UNICODE, URL encoding, Base64

| Basis | Encryption | Encoding |
|---|---|---|
| Definition | It is the process to encode data securely such that only the authorized user who knows the key or password is able to retrieve the original data. For everyone else it is just garbage. | It is the process of transforming data into such a format that it can be used by a different type of system using publicly available algorithms. |
| Purpose | The purpose of encryption is to transform data to keep it secret from others. | The main purpose is the protection of the integrity of data. |
| Used for | It is used to maintain data confidentiality. | It is used to maintain data usability. |
| Reverse Process | The original data can be retrieved using decryption. | The original data can be retrieved using decoding. The algorithm used to encode the data is publicly available. |
| Key requirement | The encryption key is required to decrypt the data and get the original data. | The encryption key is not required to decrypt the data and get the original data. |
| Secure | The encrypted data is more secure. | The encoded data is less secure. It can easily be decoded. |
| Example of Algorithm | AES, RSA, and Blowfish. | ASCII, UNICODE, URL encoding, Base64. |
| Real-life example | Securely sending a password over the internet. | Viewing special characters on the web page. |

#### What is the Wassenaar Arrangement?

A multilateral export control regime governing the international transfer of conventional arms and dual-use goods and technologies.

Established: 1996-07-12 in Wassenaar, Netherlands

Purpose: to "contribute to regional and international security and stability by promoting transparency and greater responsibility", to ensure certain technologies are not transferred or otherwise diverted to countries that undermine these goals.

The list of restricted technologies is broken into 2 parts. Information security (infosec) is part of the Basic list (one of two).

Encryption is one of these technologies that is under this control.

#### One-time-pad?

From Wikipedia:

> The one-time pad (OTP) is an encryption technique that cannot be cracked in cryptography.
> It requires the use of a single-use pre-shared key that is larger than or equal to the size of the message being sent.
> In this technique, a plaintext is paired with a random secret key (also referred to as a one-time pad).
> Then, each bit or character of the plaintext is encrypted by combining it with the corresponding bit or character from the pad using modular addition.
>
> The resulting ciphertext is impossible to decrypt or break if the following four conditions are met:
>
> - The key must be at least as long as the plaintext.
> - The key must be truly random.
> - The key must never be reused in whole or in part.
> - The key must be kept completely secret by the communicating parties.

Example script:

```python
import random
import string

# include A-Z and SPACE
valid_characters = ' ' + string.ascii_uppercase

# the key must never be reused in whole or in part
def get_key(plaintext):
    key = ''
    # key needs to be as long or longer than the plaintext
    for c in plaintext:
        # the key must be random
        random_int = random.randint(0, len(valid_characters) - 1)
        key += str(valid_characters[random_int])
    return key

def get_character_index(c):
    return valid_characters.find(c)

def get_ciphertext(plaintext, key):
    cyphertext = ''
    for i in range(0, len(plaintext)):
        pc = plaintext[i]
        kc = key[i]
        pci = get_character_index(pc)
        kci = get_character_index(kc)
        # (plaintext + key) mod length of valid_characters
        cyphertext_index_value = (pci + kci) % len(valid_characters)
        cyphertext += valid_characters[cyphertext_index_value]
    return cyphertext

def get_plaintext(cyphertext, key):
    plaintext = ''
    for i in range(0, len(cyphertext)):
        cc = cyphertext[i]
        kc = key[i]
        cci = get_character_index(cc)
        kci = get_character_index(kc)
        # (cyphertext - key) mod length of valid_characters
        plaintext_index_value = (cci - kci) % len(valid_characters)
        plaintext += valid_characters[plaintext_index_value]
    return plaintext

plaintext = input('Enter a plaintext (A-Z): ').upper()
key = get_key(plaintext)
cyphertext = get_ciphertext(plaintext, key)
decrypted_plaintext = get_plaintext(cyphertext, key)

print('Plaintext:', plaintext)
print('Key:', key)
print('Cyphertext:', cyphertext)
print('Decrypted plaintext:', decrypted_plaintext)
```

## U2P18-19: Enigma Machine

Built by the Germans during the second world-war.

- Encryption & decryption machine
- Essentially a complex, automated substitution cipher
- Cracked due to a security flaw
  1. A letter was not allowed to be encrypted to the same letter, which made it possible to find the possible initial state
  2. The starting position was never truly random due to human interaction, making it possible to reverse engineer the router wirings

## U2P20-22: Emerging Technologies

### How did Enigma work?

- Rotors have different wiring connecting input to output
- Rotors move after each keypress
- The key is the initial position of the three rotors

### Cryptanalysis & brute force

- Practice of analyzing and breaking cryptography
- Resistance to cryptanalysis is directly proportional to the key size
- Cracking PRNG (Pseudo Random Number Generators)
- Variety of methods for safeguarding keys (Key Management)

### Current trends

<https://www.microsoft.com/en-us/research/blog/research-trends-in-privacy-security-and-cryptography/>

- Cloud providers play bigger role
- Homomorphic encryption
- BYOE (Bring Your Own Encryption)
- Encryption & key management
- DevSecOps
- Quantum-safe cryptography
  - [Post-Quantum Cryptography: the Good, the Bad, and the Powerful](https://www.youtube.com/watch?v=uE_Y1C4QPU8)
  - [The Journey Towards Quantum Resistant Algorithms - NIST's Initiative](https://www.youtube.com/watch?v=vWJS62eIVxI)

## More resources

- [Diffie-Hellman Key Exchange](https://www.youtube.com/watch?v=YEBfamv-_do)
- Cryptography: The Key to Digital Security, How It Works, and Why It Matters, by Keith Martin
