# Unit 5: Cyber Threats & Attack Vectors

## Summary

- Common cyber threats
- Attack vectors
- Cyber adversaries
- Malware & vulnerabilities
- Best defenses

## U5P1: Unit Introduction

Learning outcomes:

- Common Cyber Threats
- Attack Vectors
- Cyber Adversaries
- Malware and Vulnerabilities
- Best Defenses

## U5P2: Cybersecurity Threats

> Definition: The possibility of an unwelcome event happening, which could ultimately harm and interfere with an organization's operational and functional activities.

Cyber threats can be exploited by attackers to infiltrate systems and steal data, including individuals' personal information, financial details, and login credentials.

### Threat sources

Natural:

- Fires
- Floods
- Power failures

Unintentional:

- Unskilled administrators
- Accidents
- Lazy/Untrained employees

Intentional:

- External:
  - Hackers
  - Criminals
  - Terrorists
  - Foreign intelligence agents
  - Corporate raiders
- Internal:
  - Disgruntled employee
  - Service providers (they could've been attacked)
  - Contractor (they could've be attacked)

### Threat actors

| Actor | Motivation |
|---|---|
| Nation-states | Geopolitical |
| Cybercriminals | Profit |
| Hacktivists | Ideological |
| Terrorist groups | ideological violence |
| Thrill-seekers | Satisfaction |
| Insider threats | Discontent |

### Threat actors/agents

- Insider: Employee or trusted person who has access to critical access.
- Criminal Syndicates: Organised, planned and prolonged criminal activities.
- Organised Hackers: Hardened criminals who use services and botnets to perform various cyber-attacks.

### Threat Vectors

> Definition: The medium through which an attacker gain access to a system.

- Direction access
- Removable media
- Wireless
- Email
- Cloud
- Ransomware/malware
- Supply chain
- Business partners

### Activity

Take 10 mins to review the latest State of Ransomware Report:

[The State of Ransomware 2025](https://www.blackfog.com/the-state-of-ransomware-2025/)

## U5P3: Malware

Malware, or malicious software, is an all-encompassing term for software that
intentionally inflicts damage on its users who typically have no idea that they are running it.

Software that is specifically designed to disrupt, damage, or gain unauthorized access to a computer system.

Perform functions such as stealing, encrypting or deleting sensitive data, altering or hijacking core computing functions and monitoring users' computer activity.

- **Who is vulnerable to an attack:** Any individual or organization using hardware or software on a private or public network.
- **How is an attack prevented:** Minimize risk by:
  - Patch management
  - Anti-virus & firewall (software that detect and block malware)
  - Vulnerability management (update your systems)
  - User awareness (even you family members)
  - Backups
  - IDS (Intrusion Detection System) & IPS (Intrusion Prevention System)
  - MFA
  - Incident planning & management

### How? Why?

- Malware can get into a computer through a variety of mechanisms (exploiting a combination of human & technical factors)
- Attack browsers & track websites visited
- Slow down systems & degrade system performance
- Cause hardware failure (rendering computers inoperable)
- Steal personal information (including contacts)

### How Malware gets in

1. Instant messenger applications
2. Portable hardware media/removable devices
3. Browser & email software bugs
4. Untrusted sties & freeware web applications/software
5. Downloading files from the Internet
6. Email attachments
7. Installation by other malware
8. Bluetooth & wireless networks

### Malware Distribution Techniques

- **Black hat SEO (Search Engine Optimization):** Ranking malware page highly in search results
- **Social engineered click-jacking:** Tricking users into clicking on innocent-looking webpages
- **Spear-phishing sites:** Mimicking legitimate institutions to steal login credentials
- **Malvertising:** Embedding malware in ad-networks that display across hundreds of legitimate, high-traffic sites
- **Compromised legitimate websites:** Hosting embedded malware that spread to unsuspecting visitors
- **Drive-by downloads:** Exploiting flaws in browser software to install malware just by visiting a web page
- **Spam emails:** Attaching the malware to emails and tricking victims to click the attachment

### Types of Malware

- Trojans
- Viruses
- Ransomware
- Computer worms
- Rootkits
- PUAs (Potentially Unwanted Application) and greyware
- Spyware
- Keylogger
- Botnets
- Fileless malware

## U5P4: Trojans & Viruses

### Trojan

- Disguises itself as an entirely legitimate program but behind the scenes it is causing damage
- A computer program that has a hidden malicious function that evades security mechanisms, sometimes by exploiting legitimate authorizations of a system entity that invokes the program
- Unlike viruses and worms, Trojans are not self-replicating, they rely on their apparent usefulness to spread between computers.
- RAT (Remote Access Trojan) (backdoor)

#### Trojan uses

- Delete or replace critical operating system files
- Record screenshots, audio & video of victim’s device
- Use victim’s device for spamming email messages
- Download spyware, adware & malicious files
- Disable firewalls & antivirus
- Create backdoors to gain remote access
- Steal personal information such as passwords, security codes, & credit card information
- Encrypt data & lock out the victim from accessing their devices

### Viruses

> A computer program that can replicate itself, infect a computer without permission or knowledge of the user, and then spread or propagate to another computer.

Generally transmitted through:

- File downloads
- Infected disk/flash drives
- As email attachments

#### Characteristics

- Infect other programs
- Transform themselves
- Encrypt themselves
- Alter data
- Corrupt files and programs
- Self-replicate

#### Viruses uses

- Inflict damage on devices
- Realize financial benefits
- Vandalize intellectual property
- Practice hacking skills
- Engage in cyber terrorism
- Distribute political messages
- Damage networks or computers
- Gain remote access

#### Lifecycle

1. **Design:** developing virus code (this is mostly outsourced and payed for)
2. **Replication:** for a period within the target system and then spreading
3. **Launch:** activated when user performs certain actions
4. **Detection:** identified as a threat infecting target system
5. **Incorporation:** antivirus software developer assimilate defenses against the virus
6. **Execution of the damage routine:** users install antivirus updates and eliminate the virus threats

#### Ways to get infected

- Accepting files & downloads from unverified sources
- Opening infected email attachments
- Installing pirated software
- Not updating software
- Not running latest endpoint protection
- Clicking malicious ads online
- Using portable media
- Connecting to untrusted networks

## U5P5: Ransomware

> When the attacker encrypts the files on a user's computer and then a link comes up asking for money to release the files.

- Recent ransomware both takes down the system and holds client data hostage (for example the [HSE attack](https://www.hse.ie/eng/services/publications/conti-cyber-attack-on-the-hse-full-report.pdf))
- Often decryption tools don’t recover all data.
- [ENISA Ransomware Report](https://www.enisa.europa.eu/publications/enisa-threat-landscape-for-ransomware-attacks)

### Attack chain

- Gaining access
  - Phishing
  - Getting credentials
  - Utilizing vulnerabilities
- Preparation
  - Command & control
  - Lateral movement (browsing the system undetected)
  - Privilege escalation
- Impact
  - Data theft
  - Encryption

### When you're hit by ransomware

If you don't already have plans or routines within your organization:

- Isolate system
- ID the malware
- Involve authorities
- Involve experts
- Remove malware
- Recover with decryption
- Recover data
- Prevent further attack

### What is ransomware?

Ransomware is a form of malware that encrypts a victim's files. The attacker then demands payment from the victim to restore access to the data. Victims are shown instructions for how to pay a fee to get the decryption key.

### How to prevent ransomware?

1. Backup essential files: always have a safe and up to date back.up which is kept separate from the network or computer system
2. Anti-virus updates: only use official sources to update your antivirus software and computer systems
3. Links and attachments: Do not open attachments or links unless you know and trust the source
4. Data organization: do not mix data from your work and personal online activity
5. Remote access: be careful when using remote access methods to your company network
6. Report any attack and do not engage: If you're a victim of a ransomware, report it to your local Garda station immediately

## U5P6: Worms

- Memory-resident, stand-alone malware that replicate themselves without the need for hosts in order to spread.
- Often propagate over connections by exploiting security vulnerabilities on target computers and networks.
- The primary effect of the of computer worm is to rapidly consume network bandwidth as the worm replicates.
- May also be able to crash an operating system or server application (performing a DoS (Denial of Service) attack).
- Like viruses, worms can carry a payload that may perform some other malicious action such as installing a backdoor.

### Rootkit

- Programs that hide their presence as well as attacker’s malicious activities, granting them full access to the server or host at that time, and in the future
- Rootkits replace certain operating system calls and utilities with their own modified versions, undermining the security causing malicious functions to be executed
- A typical rootkit comprises or backdoor programs, DDoS programs, packet sniffers, log-wiping utilities, IRC bots, etc.

### PUA (Potentially Unwanted Application)

> Also known as greyware or junkware. Potentially harmful applications that may pose sever risks to the security and privacy of data stored in the system where they are installed
>
> Installed when downloading and installing freeware using a third-part installer or when accepting a misleading license agreement
>
> Covertly monitor and alter the data or settings in the system

Types of PUAs:

- Adware
- Torrent
- Marketing
- Cryptomining
- Dialer

### Adware

> Software or program that supports advertisements and generates unwanted ads and pop-ups
>
> Tracks the cookies and user browsing patterns for marketing purposes and collects user data
>
> Consumes additional bandwidth, and exhausts CPU resources and memory

Indications of Adware:

- System lag
- Spammy Ads
- System crash
- Conflicting browser homepage
- New toolbar or
browser add-ons
- Slow internet

### Spyware

- Spyware is software that hides, and without permission, collects information from a device
- Can perform adware-like tracking
- Monitor local application activity, take screenshots, & activate recording devices (microphone/webcam)
- Another spyware technique is to perform DNS redirection to pharming sites.
- Hides its process and files to avoid detection and removal

Spyware Propagation:

- Drive-by download
- Masquerading as anti-spyware
- Web browser vulnerability exploits
- Piggybacked software installation
- Browser add-ons
- Cookies

What does it do?

- Steals users’ personal information and send it to a remote server or hijacker
- Monitors users’ online activity
- Displays annoying pop-ups
- Redirects a browser to ad sites
- Changes browser settings
- Changes firewall settings

[Pegasus, an example spyware](https://en.wikipedia.org/wiki/Pegasus_(spyware))

### Keylogger

- Records each keystroke as the user types on a keyboard
- Logs onto a file, or transmits them to a remote location
- Allows attacker to gather confidential information

### Botnets

- Collection of **compromised devices** connected to the internet to perform a distributed task (DDoS)
- Attackers distribute malicious software that turns a user’s device into a bot

> [!NOTE]
> Bot refers to a program or an infected system that performs repetitive work or acts as an agent or a user interface to control other programs

### Fileless Malware

Also know as: **APT** (Advanced Persistent Threat), **AVT** (Advanced Volatile Threat), and **LOC** (Low Observable Characteristics) attack

- A hacker leverage applications already installed in a computer
- Do not need to install malicious software or files to initiate an attack
- Difficult to detect

## U5P7: Video: Anatomy of an Attack

[Cisco - Anatomy of an IoT Attack](https://youtu.be/jK0oG-cDF4Y)

It shows how an attacker could get access to networks through using IoT (Internet of Things) devices that are easy to misjudge as safe devices connected to a network.

It also highlights how an attacker preferably gain access to the target by first infiltrating a smaller less secure target that the main target utilizes.

## U5P8: Zeroday & Vulnerabilities

> [!NOTE]
> Zeroday malware
> Any malware that exploits a vulnerability not previously known to the public or to the vendor of the technology containing the vulnerability.
> Commercial purveyors of zero day malware have been known to charge over $1 million for a single exploit.
>
> Example is [Stuxnet](https://en.wikipedia.org/wiki/Stuxnet).

### What is Vulnerability?

The existence of a weakness in an asset that can be exploited by threat agents.

- Hardware or software misconfiguration
- Insecure or poor design of the network or application
- Inherent technology weakness
- Careless approach of end users

Common Vulnerabilities:

- **Users:** Intentional or unintentional human errors may affect the security of web servers, application platforms, databases, and networks (the user should actually not be at blame, but the system the user uses)
- **Operating systems:** Buffer overflows, bugs in the OS, or unpatched OS
- **Applications vulnerabilities:** in applications often lead to sensitive information disclosure, cross-site scripting, session hijacking etc.
- **Network devices:** Failing to change default settings etc.

Vulnerability Classification:

- Misconfigurations/Weak configurations
- Default installations/default configurations
- Application flaws
- Poor patch management
- Design flaws
- Operating system flaws
- Default passwords
- Zero-Day vulnerabilities
- Legacy platform vulnerabilities
- System sprawl/undocumented assets
- Improper certificate and key management
- Third-party risks

## U5P9: Malware Guidance Activity

Download each of these links and review.

- [NCSC Cyber Vitals Checklist](https://www.ncsc.gov.ie/pdfs/Cyber_Vitals_Checklist.pdf): Great checklist to check if your organization follows vital security standards
- [Break the chain](https://www.ncsc.gov.ie/pdfs/NCSC_Quick_Guide_Ransomware.pdf): Informs how a ransomware attack is generally done, and also how to prevent it by:
  - Reduce attack surface
  - Patching
  - MFA
  - Logging & monitoring
  - Backups
  - Have a plan
  - User awareness
- [Malware Guidance](https://www.ncsc.gov.uk/guidance/mitigating-malware-and-ransomware-attacks): How to mitigate malware and ransomware attacks
  - 4 action to take:
    - Action 1: make regular backups
    - Action 2: prevent malware from being delivered and spreading to devices
    - Action 3: prevent malware from running on devices
    - Action 4: prepare for an incident
  - Steps to take if your organization is already infected
    - Disconnect from all network connections
    - Turning off your Wi-Fi, disable core network connections, and disconnect to the internet
    - Reset credentials (without locking yourself out)
    - Wipe & reinstall the infected devices
    - Only restore a backup that is verified to be free from malware
    - Connect to clean network and install/update OS and software
    - Install/Update/Run antivirus software
    - Reconnect to the network
    - Monitor and run antivirus scans
  - Great resource of known decryption tools to decrypt encrypted data affected by ransomware attacks: [No More Ransom Project](https://www.nomoreransom.org/en/index.html)
- [ENISA Threat Landscape for Ransomware Attacks](https://www.enisa.europa.eu/publications/enisa-threat-landscape-for-ransomware-attacks): A more in-depth report about ransomware attacks, what it is and how it's executed

## U5P10: Notable Attacks Activity

- Conti (HSE)
- DarkSide (US Pipeline)
- NotPetya
- StuxNet
- WannaCry
- CryptoLocker
- Mirai botnet
- Mydoom
- ILOVEYOU
- Emotet

[11 real and famous cases of malware attacks](https://gatefy.com/blog/real-and-famous-cases-malware-attacks/)

Choose 2 attacks research.

- Who?
- What?
- Where?
- When?
- Why?
- Ransomware?
- Ransom Paid?
- Impact?
- Still operating?
- State involvement?
- Actors, infection vector, impact etc

## U5P11: Protect from Attack

- Install protection software
- Backup data and systems
- Have an incident response plan in place (and test it)
- Carry out regular security awareness training (make it fun)
- Monitor networks in real time (you'll never find a vulnerability if you're not looking for it)
- Regular vulnerability patching & updates
- Practice caution when working with files/email from unknown sources
- Download files only from reputable Internet sites
- Install firewall, IPS, IDS
- Scan your hard drive for viruses regularly

### Anti-Virus Software

> Aims to detect, isolate and if necessary, delete malware on a computer before it can harm data.
>
> Uses several techniques to identify malware, the two most common are known as **signatures** and **heuristics**.

- Signatures: A malware’s signature is a distinctive pattern of data either in memory or in a file. This can be identified by anti-virus software. Polymorphic viruses avoid this detection.
- Heuristics: Complementing signatures, heuristics use rules to identify viruses based on previous experience of the behaviour of known viruses. Unidentified malware can be detected by their behaviour

### Cyber Incident Response Plan

- Prepare for the worst
- Reduce the impact
- Enhance the recovery
- When, not if

[Public Sector Cyber Security Baseline Standards (Nov 2021)](https://www.ncsc.gov.ie/pdfs/Cyber_Security_Baseline_Standards.pdf)

### Actions

- Backup strategy (3-2-1-1-0 rule: 3 backups, on 2 medias, 1 of them offsite, 1 immutable, air-gapped, 0 failures ([The 3-2-1 Rule Is Dead: Here’s Why We Need 3-2-1-1-0](https://backupcentral.com/the-3-2-1-rule-is-dead-heres-why-we-need-3-2-1-1-0/)))
- Security controls & hardening
- MFA
- Employee training & awareness
- Plan, plan, plan!
- Implement framework
- Don't pay ransom
