# Unit 3: Identity & Access Management (IAM)

## Summary

In this unit we covered:

- IAM
- Authentication
- Authorization
- Passwords

## U3P1: Unit Introduction

Learning outcomes:

- Understand terminology, principles & types of access control
- Overview of IAM
- Understand user access management
- Understand the different types of authentication
- Understand different types of authorization
- Understand user accounting

We'll learn about different ways of identifying individuals, authorizing them, and passwords

## U3P2-P3: IAM & Authentication

IAM responsible for providing the right individual with the right access at the right time

- Authentication
- Authorization
- Identity Management
- Identity Repository

### Access control

- Allowing only authorized entities to observe/modify/take possession of a computer system or physical property
- Subject: person, system, or process
- Object: entity being accessed
- Limit access by using rules/roles/labels

### Type of access control services

| Access Control Service | Description |
|---|---|
| IAM | Unique identifier for each subject (username/email), includes methods to ensure identity (authentication/login), usually administered with Identity Management System |
| Authorization |  Determines capabilities or rights of the subject |
| Audit | Logs or records of system activities |
| Accountability | Reports/reviews logs, and connect them to the correct individuals |

### Identity management

- Control users/entities in system (account names, passwords, profiles, access rights)
- Consider identity within context of interconnected systems
- Make sure the individuals get the correct access, and minimizing that any get incorrect access

#### Process

Identification > Authentication > Authorization

### Identification types

| Identification Type | Description |  |
|---|---|---|
| ID Cards/Badges | Physical device with subject’s picture, name, other characteristics. | Vulnerable to social engineering attacks (can be copied or re-created) |
| User IDs | String of characters, unique to one individual. (random user IDs are more secure than using emails) | Vulnerable to social engineering attacks and shoulder surfing |
| Email Address | Often used as a user ID, particularly for web commerce sites because it is globally unique. | Reused everywhere, so easier to spoof, and there's no restrictions preventing someone else using another's email |
| Account Number/PIN | Provides a unique identifier for a specific user within a system. | Difficult to remember, PINs are usually short and easy to brute force, usually people use personal info as a basis of PINs |
| MAC Address | 48-bit number that uniquely identifies a computer. | No longer embedded in hardware but set by software, can be changed by anyone with admin access, can also be spoofed |
| IP Address | Provides the logical location of a device on a network. | Assigned by software, can be identical across subnets, can be spoofed |
| RFID Tag | Uses radio signals to track people and devices | listen to any request signal without verifying, can be spoofed using a Flipper Zero |

### Authentication types

Can you prove that you are who you say you are? Methods:

- Something you **know** (password, passphrase, PIN, graphical password)
- Something you **have** (some physical device, magnetic stripe cards, smarts cards, tokens)
  - 2FA is a combination of something you know and have
- Something you **are** (fingerprints, hand geometry, retina scans, iris scans, facial recognition, voiceprints)
  - Behavioral device (keystroke recording, touch screen movement, signatures)

### Password administration

- Administrative policy
- Backed by technical policy
- Balance between more frequent (more likely to be written down) and less frequent (more likely password-cracking will work) required password change
- Users must protect passwords
- Admins should not know users passwords

> [!NOTE]
> Minimum days to be allowed to set a new password can be used to prevent users to change passwords enough times to go over a limit so they then can essentially re-use an old password.

### Biometric acceptance

Some are more accepted by people, like fingerprints, voice analysis, facial recognition.

While some raise concerns by people, like when it invades civil liberty, makes it difficult to sanitize scanner, or is a health concern.

All system can fail; test periodically

We want to avoid a high FRR (False Rejection Rate) or FAR (False Acceptance Rate), which can be tuned by the sensitivity (more sensitive = higher FRR, less sensitive = higher FAR).

### Multi-factor

Multi-factor can be more than 2 factors.

Two-factor authentication example: The user enter their login credentials (username & password), a code/token is sent to the user's device, and the user enter this to log in.

[What is Two-Factor Authentication? (2FA)](https://www.youtube.com/watch?v=0mvCeNsTa1g)

## U3P4-P5: SS0 (Single Sign-On) and "Weak! Who are you?" Video

Allows a user to authenticate themselves to multiple servers on a network with a single password
without re-entering it every time.

- No need to remember passwords of multiple applications or systems
- Reduces the time for entering a username and password
- Reduces the network traffic to the centralized server Users need to enter credentials only once
for multiple application
- Users need to enter credentials only once for multiple devices

### Administrative Management Controls

- **Separation of duties:** assigns parts of tasks to different individuals thus no
single person has total control of the system’s security mechanisms; prevent
collusion
- **Least privilege:** a system’s user should have the lowest level of rights and
privileges necessary to perform their work and should only have them for the
shortest time.
  - Three types: Read only, Read/write and Access/change
- **Two-man control:** two persons review and approve the work of each other, for
very sensitive operations
- **Dual control:** two persons are needed to complete a task
- **Rotation of duties:** limiting the amount of time a person is assigned to perform
a security related task before being moved to different task to prevent fraud;
reduce collusion
- **Mandatory vacations:** prevent fraud and allowing investigations, one week
minimum; kill processes
- **Need to know:** the subject is given only the amount of information required to
perform an assigned task, business justification
- **Agreements:** NDA, no compete, acceptable use

### Accountability

- Identification must support the ability to tie an action back to an entity.
- Authentication must be strong:
  - A perpetrator of account abuse can't shift blame to weak
authentication practices.
- Training and awareness must be available and mandated so all users:
  - Understand good account practices and penalties for account abuse.
- Continuous monitoring:
  - Ensures account abusers are quickly identified and held accountable.
- Audit logs keep a record of actions that can be traced back to users.
- Policies should support accountability so implementation is consistent and
fair.

### Authorization

Describes entity's capabilities/roles once identified and authenticated.

What this user, system, or group can access, change, or execute?

### Passwords

[Michael McIntyre Nearly Lost His Mind Trying to Remember His Password](https://youtu.be/z_HmDP3lKMI)

Humans tend to do the same things, the same with generating and managing passwords.

## U3P6-P7: Passwords Continued

### Password based authentication

- Most popular defense against intruders
- System compares with stored

### Threats

- Disclosure (it can be revealed)
- Inference (it can be assumed (or guessed))
- Exposure (it can be released)
- Loss (it can be forgotten)
- Snooping/eavesdropping
- Cracking

### How is password cracking possible?

Passwords are NOT truly random.

- 52 upper/lowercase letters, 10 digits, and
32 punctuation symbols equals ≈ 6
quadrillion possible 8-character
passwords
- People like to use dictionary words,
relative and pet names equaling ≈ 1
million common passwords
- Different systems impose different
password requirements.
- Passwords need to be changed often.
- Some passwords are only used
occasionally
- People reuse passwords

### Types of password cracking attacks

- **Dictionary Attack**
  - Quick technique that tries every word in a specific
dictionary
  - Rainbow Tables: list of hashes of popular
passwords
- **Brute Force Attack**
  - Tries all combinations of letters, numbers & symbols
- **Hybrid Attack**
  - Adds numbers or symbols to the end of a word
- **Popular programs for password cracking on Kali Linux**
  - John the Ripper
  - Brutus

### Dictionary attack

- Attacker can compute H(word) for every word in a dictionary and see if the result is in the password file
- With 1,000,000-word dictionary and assuming 10 guesses per second, brute-force online attack takes 50,000 seconds (14 hours) on average
- Offline attack much quicker

This is less of a threat when you apply rate-limits and account lock downs when failing too many times.

### Passwords & hash functions (video)

[Passwords & hash functions (Simply Explained)](https://www.youtube.com/watch?v=cczlpiiu42M)

Passwords can be saved in the DB as:

- Plaintext (super bad and easy for hackers that obtain them)
- Encrypted (better, but it can potentially be decrypted)
- Hashed (best, can't be decrypted)

#### Hash vulnerabilities

- Hashing functions are optimized to be fast, but this can also be used for brute-force attacks to quickly test potential passwords against hashes (hundred of millions per second).
  - To mitigate this, some hash functions (bcrypt, scrypt, argon2) provide a `Cost` parameter, to slow it down  
- Hashing always generates the same output from the same input, so if users share the same password it would mean that a hacker would only need to crack one of them.
  - To mitigate this, some `Salt` (random data) is added to the password before hashing, making sure it is unique.

#### Combination

You can combine all of these security measures for even better security.

For example: Dropbox generate a simple hash from the password, but then hashes the hash in a slowed down hash function like bcrypt, which is then encrypted before being save to the DB.

## U3P8: Salting Hashes

Salting requires adding a random piece of data and to the password before hashing it.

- Means that the same string will hash to different values at different times
- Users with same password have different entries in the password file
- Salt is stored with the other data as a complete hash
- Salt may be the same for all or random

### Advantages

- Prevents use of `rainbow tables`.
- With salt, attacker must compute hashes of all
dictionary words once for each password entry
  - With 12-bit random salt, same password can hash
to 212 different hash values
  - Attacker must try all dictionary words for each
salt value in the password file

### Cracking protection: iteration count

- The same password can be rehashed many
times over to make it more difficult for the
hacker to crack the password.
- This means that the precompiled dictionary
hashes are not useful since the iteration
count is different for different systems
  - Dictionary attack is still possible!

### Activity

#### Research "Three Random Words"

[The logic behind three random words](https://www.ncsc.gov.uk/blog-post/the-logic-behind-three-random-words)

- What is it: an easy standard to adopt to generate more secure and rememberable passwords
- How does it work: think of 3 random words and combine them into 1 password
- What does the research say: it generates longer, more memorable, secure, & diverse passwords, and the standard is also designed to be easy to explain and understand
- Are you convinced: yes, but combining this with password managers and using passphrases is even better

#### Research "No Forced Password Change"

Mentioned in [NIST guideline](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-63B-4.pdf) att section 3.1.1.2, which talks about passwords requirements.

- What is it: it questions the policy of forcing password changes after a period of time
- How does it work: password changes are instead only required if the password has been compromised
- What does the research say: forcing password changes often leads to weaker passwords, instead it's better to focus on requiring strong passwords
- Are you convinced: yes, it seems not only that the research backs it up, but it also makes sense

#### Research "Passwordless"

- What is it: authentication without the use of passwords (or any other knowledge-based secrets)
- How does it work: the user usually provide a public identifier (e.g. username) and then a secure proof of identity through a device or token. Typically a key-pair is used (saving the public key on the service, and the private key on the user's device), so that a biometric signature can be used
- What does the research say: far safer than passwords authentication, and more user friendly
- Are you convinced: yes, it makes it easy and safe for me as a user

## U3P9: Top Passwords

[Nordpass: Most common passwords list](https://nordpass.com/most-common-passwords-list/)

[haveibeenpwned: Check if your email, phone or password is in a data breach](https://haveibeenpwned.com/)

## U3P10: Policy

- If possible, use MFA
- Use unique passwords
- If you can, use a password manager
- If you must, create your own passwords (the longer the better, passphrase is even better)

### Improving password security

- Implement a password policy in your organization. [UCD Password Policy](https://hub.ucd.ie/usis/W_HU_MENU.P_DOWNLOAD_FILE?p_filename=Password%20Protection%20Policy.pdf&p_parameters=36F8A0AC5B0D6F23FA1EEB8E7C5668E87D47F894CE813A2C5A31FE1A69D113A3E1C278129BDAF0CFDDCE3164583EBA53F9D0F7E2674DBBEE67B5312E90DE5FC3)
- Password complexity
  - Case-sensitivity
  - Use of special characters, numbers, and both upper and lower-case letters
  - Minimum length requirements: longer the better for passwords/passphrases
- Security questions
  - Ask personal questions which need to be verified
  - Some questions are very easy to discover answers
- Virtual keyboard
  - Person clicks on-screen keyboard to enter password (prevents key-logging)
- Single sign-on
  - User only has to remember one password at a time and yet can access all/most of their resources
  - AKA Enterprise Reduced Sign-On (almost impossible to have one password
used for everything due to integration issues)
- Centralized password storage management
  - Online sites accessible through one password which contain all other passwords

### Guidelines for mitigating access control attacks

#### Software-based

- Mitigate DoS attack effects with load balancing systems at key points in network.
- Encrypt passwords with strong hashing algorithm.
- Tightly control access to password hash databases.
- Use password masking.
- Test all access control software to catch memory overflow vulnerabilities.
- Install anti-malware solutions on network hosts that actively monitor for threats.
- Make sure malware definitions are always up-to-date.
- Use password policy technical controls that make brute forcing attempts unfeasible.
- Properly wipe drives with sensitive data, especially stored credentials.
- Implement vulnerability scanning/assessment for any systems likely to be target.
- Implement IDS to continuously monitor your network/hosts.

#### Socially engineered

- Train all staff to identify various social engineering attacks.
- Write a secure communications policy.
- Follow the principle of least privilege.
- Plan a social engineering pen-test
  - Test has ethical implications, so abide by rules of conduct at all times.
- Destroy all hard copy documents with sensitive information before discarding.
- Educate users on reporting suspicious behavior to IT or security team.
- Mandate use of multi-factor authentication for critical systems.

#### Human-based

- Train users as to why certain passwords are weak and easy to guess.
- Enforce account lockout policies on your systems to prevent brute-force attacks.
- Display last logon information to users.
- Lock down or isolate all sensitive hardware.
- Encrypt all sensitive information in storage and transit.
- Ensure staff can easily contact law enforcement if faced with threating behavior.

#### Physical

- Make sure all locks and doors are properly maintained.
- Routinely verify integrity of perimeter access control mechanisms (e.g., fences).
- Ensure that physical access control devices have tamper protection.
- Include hostage alarms/hostage key patterns to cipher locks/access control systems.
  - Should someone be forced to open a door under duress, a silent alarm can be triggered.
- Place surveillance cameras at key entrances and exits.
- Ensure guards/security personnel have direct access to central security/law enforcement in the event of a violent confrontation.
- Place critical hardware in access controlled rooms, safes, or lockboxes.
- Monitor equipment that would compromise operations if damaged with cameras/guards.

### Access control policies example

Start with administrative policies.

Reinforce with technical policies.

- All passwords must be at least seven characters long using three different types of characters.
- A user's identity must be verified before IT staff can reset that person's password.
- Process to suspend/deactivate user account in case of termination/compromise/infection.
- Inactive user accounts must be disabled after 60 calendar days.
- User account will be locked out for 15 minutes after three bad logon attempts.
- Users can’t have local administrative privileges on their computer unless approved by manager.
- Existing local administrative privilege will be reviewed annually.
- All administrator accounts must use two-factor authentication to log on to the network.
- All workstations must implement a screen lock after 15 minutes of inactivity.
- Access to administrator systems must be reviewed annually.
- IT staff may not use administrator accounts for general purpose.
- Vendor and contractor access list to be approved, monitored, and limited to the length of the contract.
- Default administrator passwords must be changed before the system goes into production.
- Default ports for administrator access must be changed when possible.
- Administrative access cannot be accomplished through a public interface.
- Each new user account will receive a unique first-time password that must be changed upon first use.
- Any reset passwords must be set to unique value for each user and changed upon first use.

## U3P11-P12: Password Cracking

[Password Cracking - Computerphile](https://www.youtube.com/watch?v=7U-RbOKanYs)

### Kali Linux

- Suite of digital forensic and pen testing
tools
- Best run on a virtual machine
- Excellent learning resource

[Kali Tools documentation](https://tools.kali.org/tools-listing)
[Get Kali](https://www.kali.org/get-kali/)
