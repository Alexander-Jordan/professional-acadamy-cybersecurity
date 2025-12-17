# Unit 6: Security Technologies & Controls

## U6P1: Unit Introduction

Learning outcomes:

- Network Security
- Application Security
- Cloud Security
- Mobile, IoT and OT Security

## U6P2-3: Video "Anatomy of a Cyber Attack"

[Cyber Ireland: Anatomy of a Cyber Attack Video](https://youtu.be/pXoLcDvTSac)

> [!NOTE]  
> [Checkpoint: Live cyber threat map](https://threatmap.checkpoint.com/)

### Anatomy of a cyber attack

1. Reconnaissance
2. Weaponization
3. Delivery
4. Exploitation
5. Installation/C&C
6. Action on objective

### Defending against a cyber attack

1. Perimeter security
2. Network security
3. The human layer
4. Endpoint security
5. Application/Log security
6. Data security

## U6P4: Anatomy of an Attack Continued

### Kill chain: the 7 stages of a cyber attack

1. Reconnaissance: scanning the environment or harvesting information from social media
2. Weaponization: pairing malicious code with an exploit to create a weapon (piece of malware)
3. Delivery: transmission of weapon/malware to target (e.g. via email, USB, website)
4. Exploitation: once delivered, the weapons/malware code is triggered upon an action. This in turn exploits the vulnerability
5. Installation: the weapon install malware on the system
6. Command & control: a command channel for remote manipulation of the victim
7. Action on objectives: with hands on access the attacker achieve their objective

### Security Challenges

- Compliance to government laws and regulations
- Lack of qualified and skilled cybersecurity professionals
- Difficulty in centralizing security in a distributed computing environment
- Fragmented and complex privacy and data protection regulations
- Compliance issue due to the implementation of BYOD (Bring Your Own Device) policies in companies
- Relocation of sensitive data from legacy data centres to the cloud without proper
configuration

### Impact of Information Security Attacks

- Financial Losses
- Loss of confidentiality and integrity
- Damaged customer relationship
- Loss of business reputation
- Legal and compliance issues
- Operational impacts

### Network Security Principles

- Network Security Controls
- Network Security Protocols
- Network Security Devices

### Network Defense Benefits

- Protect information assets
- Comply with government and industry specific regulations
- Ensure secure communication with clients and suppliers
- Reduce the risk of being attacked
- Gain competitive edge over competitor by providing more secure services

### Network Defense Challenges

- Distributed Computing Environments:
  - With the advancement in modern technology and to meet business requirements, networks are becoming vast and complex, potentially leading to serious security vulnerabilities. Attackers exploit exposed security vulnerabilities to compromise network security
- Emerging Threats:  
  - Potential threats to the network evolve each day. Network security attacks are becoming technically more sophisticated and better organized
- Lack of Network Security Skills:
  - Organizations are failing to defend themselves against rapidly increasing network attacks due to the lack of network security skills

### Network Defense Approaches

- Preventive Approaches
  - Consist of methods or techniques that are used to avoid threats or attacks on the target network
- Reactive Approaches
  - Consist of methods or techniques that are used to detect attacks on the target network
- Retrospective Approaches
  - Consist of methods or techniques that examine the causes for attacks, and contain, remediate, eradicate, and recover from damage caused by the attack on the target network
- Proactive Approaches
  - Consist of methods or techniques that are used to make informed decisions on potential attacks in the future on the target network

### Administrative Security Controls

Examples:

- Regulatory Framework Compliance
- Security Policy
- Employee Monitoring & Supervising
- Information Classification
- Security Awareness & Training

### Physical Security Controls

Examples of physical access controls:

- Locks
- Fences
- Badge system
- Security guards
- Mantrap doors
- Biometric system
- Lighting
- Motion detectors
- Closed-circuit TVs
- Alarms

### Technical Security Controls

- Access Controls
- Authentication
- Authorization
- Auditing
- Security protocols
- Network Security Devices

## U6P5-6: Network Segmentation/NIST CS and Video

### Network Segmentation

A network that could be partly closed off, to not impact other segments in the network in case of an attack.
It's also for better performance.

Benefits:

- Improved Security
- Better Access Control
- Improved Monitoring
- Improved Performance
- Better Containment

### What is a Firewall?

[What is a firewall and why do I need one?](https://www.techtarget.com/searchsecurity/definition/firewall)

> A firewall is a network security device that prevents unauthorized access to a network.
> It inspects incoming and outgoing traffic using a set of security rules to identify and block threats.

### DMZ (Demilitarized Zone)/Perimeter Network Architecture

[Wikipedia: DMZ (computing)](https://en.wikipedia.org/wiki/DMZ_(computing))

> A physical or logical subnetwork that contains and exposes an organization's external-facing services to an untrusted, usually larger, network such as the Internet.
> An external network node (eg the Internet) can access only what is exposed in the DMZ, while the rest of the organization's network is protected behind a firewall.
> The DMZ functions as a small, isolated network positioned between the Internet and the private network.

### IDS (Intrusion Detection Systems)

Compared to IPS, IDS doesn't block the attacker, just detecting.

- Hardware/software that passively monitors for potential attacks
- Technical/Detective control
- Monitors for:
  - Known malicious patterns of activity
  - Detect new activities not previously seen
- Monitoring based on:
  - Ports
  - Protocols
  - Application payload types
  - Authentication attempts
  - File access
  - Privilege use on single host

### IPS (Intrusion Prevention System)

Compared to IDS, IPS blocks the attacker.

- IDS that proactively responds to potential attacks
- Technical/Preventive control
- Inserted inline into traffic stream
- Any traffic that violates restrictions in signature file/anomaly database is blocked
- Often integrated into firewalls or unified threat management systems

### IDS/IPS Detection Methods

- Signature-based
  - Uses predefined set of rules to identify unacceptable traffic
  - Must periodically update signature file provided by vendor
- Anomaly-based
  - Compares activity with a baseline of acceptable patterns
  - “Learns” what is normal when installed
  - Dynamic
  - Administrator can also add acceptable patterns to the database.
- Many modern systems are hybrid

### SIEM (Security Information and Event Management)

[IBM: What is SIEM?](https://www.ibm.com/think/topics/siem)

Rapidly developed with AI.

- Collection and analysis of security event logs
  - Servers
  - Routers
  - IDS
  - IPS
- Correlates events and issues notifications to central console
- Used for vulnerability management and compliance tool
- Big Data is becoming a popular replacement for SIEM:
  - Mining and analysing security events
  - Spotting trends
  - Predicting security breaches before they happen
  - Gleaning hard-to-discover information out of vast stores of security and system log information

### Defense in depth

[Imperva: Defense-in-Depth](https://www.imperva.com/learn/application-security/defense-in-depth/)

> Defense-in-depth is an information assurance strategy that provides multiple, redundant defensive measures in case a security control fails or a vulnerability is exploited.

Illustration: an egg (old security), an onion (todays security).
Not only one layer of defense.

Layer | Types of protection
---|---
Perimeter security | Firewall, IDS/IPS, DMZ, Message security, Honeypot, DLP, DHS einstein
Network security | Firewall, IDS/IPS, VoIP protection, Inline patching, Web proxy content filtering, NAC, Message security, Wireless security, Remove access, DLP
Endpoint security | Firewall, IDS/IPS, Content security, Endpoint security enforcement, FDCC compliance, Patch management, DLP
Application security | Static app testing/code review, Dynamic app testing, WAF, Database monitoring/scanning, Database secure gateway (shield)
Data security | PKI, Data wiping cleansing, Identity & access management, Enterprise right management, Data classification, Data integrity monitoring, Data/Drive encryption, DLP
Policy management (prevention) | It security governance, Security policies & compliance, Security architecture & design, Continuos C&A, Cyber threat intelligence, Threat modelling, Risk management, Security awareness training, Penetration testing, Vulnerability assessment
Operations (monitoring & response) | SIEM, Escalation management, Focused OPS, Digital forensics, Continuos monitoring & assessment, Situational awareness, SOC/NOC monitoring, CIRT, Security dashboard, Security SLA/SLO reporting

Device | Application | Computer | Network |Physical | Policies, procedures & awareness

### Guidelines for Implementing Network Components Security

- Harden routers, switches, firewalls, and other networking components (disable what you're not using)
- Use VLANs to partition your network and segregate traffic
- Use physical network partitioning in high-security environments
- Use firewalls to protect your internal network from the Internet
- Deploy public-facing servers (web/email/DNS) in a DMZ or perimeter network
- Lock down remote access server with same care you would give to your firewall
- Use endpoint security to provide comprehensive protection for (and from) remote users
- Ensure CDN is protected against:
  - Malware
  - Insufficient input validation
  - Poor session management
- Educate users to not automatically accept content with self-signed certificates
- Secure any non-computer physical devices against tampering or accidents

### NIST CSF 2.0

> [!NOTE]  
> Not the same as NIS

[NIST: The NIST Cybersecurity Framework (CSF) 2.0 is Here!](https://csrc.nist.gov/news/2024/the-nist-csf-20-is-here)

The update version has the `Govern` part added.

You don't have to implement the whole framework, but improve parts you need to.

### CIS (Center of Internet Security) controls (video)

[CIS Critical Security Controls](https://www.cisecurity.org/controls)

> The CIS Critical Security Controls (CIS Controls) are a prescriptive, prioritized, and simplified set of best practices that you can use to strengthen your cybersecurity posture.

[Strengthen Cybersecurity Posture with the CIS Critical Security Controls](https://www.youtube.com/watch?v=6OqnCxdncX4)

### CIS (activity)

Review CIS controls: [CIS Critical Security Controls](https://www.cisecurity.org/controls)

1. Inventory and Control of Enterprise Assets
2. Inventory and Control of Software Assets
3. Data Protection
4. Secure Configuration of Enterprise Assets and Software
5. Account Management
6. Access Control Management
7. Continuous Vulnerability Management
8. Audit Log Management
9. Email and Web Browser Protections
10. Malware Defenses
11. Data Recovery
12. Network Infrastructure Management
13. Network Monitoring and Defense
14. Security Awareness and Skills Training
15. Service Provider Management
16. Application Software Security
17. Incident Response Management
18. Penetration Testing

[CIS Control v8.1 PDF](https://learn.cisecurity.org/cis-controls-v8_1_guide_pdf)

> Note that the CIS Controls are licensed under a [Creative Commons Attribution-Non-Commercial-No Derivatives 4.0 International Public License](https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode).
