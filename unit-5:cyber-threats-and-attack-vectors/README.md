# Unit 5: Cyber Threats & Attack Vectors

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
