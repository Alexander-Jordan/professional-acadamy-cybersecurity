# Unit 2: Cryptography & Encryption

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
