# Unit 6: Security Technologies & Controls

## Summary

- Network Security
- Application Security
- Cloud Security
- Mobile, IoT and OT Security

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
--- | ---
Perimeter security | Firewall, IDS/IPS, DMZ, Message security, Honeypot, DLP, DHS einstein
Network security | Firewall, IDS/IPS, VoIP protection, Inline patching, Web proxy content filtering, NAC, Message security, Wireless security, Remove access, DLP
Endpoint security | Firewall, IDS/IPS, Content security, Endpoint security enforcement, FDCC compliance, Patch management, DLP
Application security | Static app testing/code review, Dynamic app testing, WAF, Database monitoring/scanning, Database secure gateway (shield)
Data security | PKI, Data wiping cleansing, Identity & access management, Enterprise right management, Data classification, Data integrity monitoring, Data/Drive encryption, DLP
Policy management (prevention) | It security governance, Security policies & compliance, Security architecture & design, Continuos C&A, Cyber threat intelligence, Threat modelling, Risk management, Security awareness training, Penetration testing, Vulnerability assessment
Operations (monitoring & response) | SIEM, Escalation management, Focused OPS, Digital forensics, Continuos monitoring & assessment, Situational awareness, SOC/NOC monitoring, CIRT, Security dashboard, Security SLA/SLO reporting

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

## U6P8: Cloud Computing

ISO/IEC definition:

> Paradigm for enabling network access to a scalable and elastic pool of shareable physical or virtual resources with self-service provisioning and administration on-demand.

NIST definition:

> Cloud computing is a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources (e.g. networks, servers, storage, applications, and services) that can be rapidly provisioned and released with minimal management effort or service provider interaction.

Another simpler definition:

> It takes a set of resources, such as processors and memory, and puts them into a big pool (in this case, using virtualization). Consumers ask for what they need out of the pool, such as 8 CPUs and 16 GB of memory, and the cloud assigns those resources to the client, who then connects to and uses them over the network. When the client is done, they can release the resources back into the pool for someone else to use.

Essential characteristics:

- Broad network access
- Rapid elasticity
- Measured service
- On-demand self-service
- Resource pooling

Service models:

- SaaS (Software as a Service)
- PaaS (Platform as a Service)
- IaaS (Infrastructure as a Service)

Deployment models:

- Public
- Private
- Hybrid
- Community

### Cloud service models

IaaS (Infrastructure as a Service):

- Virtualization
- Servers
- Storage
- Networking

PaaS (Platform as a Service):

- All from IaaS and:
- Runtime
- Middleware
- O/S

SaaS (Software as a Service):

- All from PaaS and:
- Applications
- Data

### Cloud Computing Benefits

Economic

- Business agility
- Less maintenance costs
- Acquire economies of scale
- Less capital expense
- Huge storage facilities for organisations

Staffing

- Streamline processes
- Efficient usage of resources
- Less personnel training
- Less IT Staff
- Multiple users can utilize cloud resources

Operational

- Flexibility and efficiency
- Resilience and redundancy
- Scale as required
- Less operational problems
- Deploy applications quickly

Security

- Less investment in security controls
- Efficient, effective, and swift response to security breaches
- Standardized open interface for MSS (Managed Security Services)
- Effective patch management and implementation of security updates
- Better disaster recovery preparedness

### Cloud Security Concerns

- Security is dependent on security practices of cloud service provider.
- User doesn’t have direct control over systems.
- Virtual machines are hosted on same computer as other customers.

### Shared Responsibility Model

The key message: even if cloud providers can take some responsibility off from the users, the users still need to understand they have a security responsibility.

**Cloud providers** should clearly document their internal security controls and customer security features so the cloud user can make an informed decision.
Providers should also properly design and implement those controls.

**Cloud users** should, for any given cloud project, build a responsibilities matrix to document who is implementing which controls and how.
This should also align with any necessary compliance standards.

### CSA (Cloud Security Alliance)

[CSA website](https://cloudsecurityalliance.org/)

> An organization that promote the use of best practices for providing security assurance within cloud computing, Artificial Intelligence and to provide education on the uses of cloud computing to help secure all other forms of computing.

### Securing the Cloud

1. Enforce data protection, backup, and retention mechanisms
2. Enforce SLAs (Service-Level Agreement) for patching and vulnerability remediation
3. Vendors should regularly undergo AICPA (American Institute of Certified Public Accountants) SAS 70 (Statement on Accounting Standards No. 70) Type II audits
4. Verify one's own cloud in public domain blacklists
5. Enforce legal contracts in employee behavior policy
6. Prohibit user credentials sharing among users, applications, and services
7. Implement strong authentication, authorization and auditing controls
8. Check for data protection at both the design stage and at runtime

## U6P9: Application Security

> Describes security measures at the application level that aim to prevent data or code within the app from being stolen or hijacked.
> It encompasses the security considerations that happen during application development and design, but it also involves systems and approaches to protect apps after they get deployed.

### OWASP (Open Web Application Security Project) Top 10

**OWASP:** A non-profit foundation that works to improve the security of software.

**OWASP Top 10:** A list of the top ten web application vulnerabilities determined by OWASP and the security community at large.

- [Top 10 2021](https://owasp.org/Top10/2021/)
- [Top 10 2025](https://owasp.org/Top10/2025/)

### Mobile Devices

- **NFC (Near-field Communication):** employs electromagnetic induction to enable communication between the devices connected within a range of 10 cm
- **Satcom (Satellite Communication):** an artificial geostationary satellite that provides services across the globe, but it is much slower and more expensive than other technologies
- **Cellular Communication:** based on a single network tower that serves devices located within a specific radius

### Connection Methods continued

- **Wi-Fi:** a common wireless technology used in homes and office buildings to connect local devices
- **Bluetooth:** a short-range, high-speed, and low-power wireless technology that enables communication between devices connected within the Bluetooth range
- **5G Cellular (Mobile) Communication:** a broadband cellular network that operates at high bandwidth with low latency and provides high-speed data down

### Mobile Device Management

- **Mobile Application Management:** a software that is mostly used by IT admins to control and secure organizational data. It offers features such as the remote activation or deactivation of devices, remote wiping in case of theft or loss, etc.
- **Mobile Content Management:** a software that offers solutions to safeguard the content or data on the mobile devices. It provides features to store and deliver data, offer the required services, and permit employees to access the organizational data remotely
- **Context-aware Authentication:** uses the contextual information of a user such as geolocation, identity, and behavior for enhancing data security decisions

### Permission Approaches

- BYOD (Bring Your Own Device)
- COPE (Company Owned, Personally Enabled)
- COBO (Company Owned, Business Only)
- CYOD (Choose Your Own Device)

#### Risks

- Sharing confidential data on unsecured networks
- Data leakage and endpoint security issues
- Improperly disposing of devices
- Supporting various devices
- Mixing personal and private data
- Lost or stolen devices
- Lack of awareness
- Ability to bypass the network policy rules of the organization
- Infrastructure issues
- Disgruntled employee

### Mobile Security Guidelines

For Security Professional:

- Use Mobile Device Management Solutions
- Implement policy around mobile device use
- Secure organizational data centres with multi-layered protection systems
- Educate employees about the COPE (Company Owned, Personally Enabled) policy
- Clarify who owns which apps and data
- Use encrypted channels for data transfer
- Clarify which apps are allowed or banned
- Control access on a need-to-know basis
- Ensure that the employees completely understand and sign-off on the policies

For Employee:

- Use the encryption mechanism to store data
- Maintain a clear separation between business and personal data
- Register devices with a remote locate and wipe facility if the company policy permits
- Regularly update the device with the latest OS and patches
- Use anti-virus and DLP (Data Loss Prevention) solutions
- Set a strong passcode for the device and change it often
- Set passwords for apps to restrict others from accessing them

## U6P10-11: Operational Technology and Video

### IoT (Internet of Things)

[Wikipedia: Internet of Things](https://en.wikipedia.org/wiki/Internet_of_things)

> Physical objects that are embedded with sensors, processing ability, software, and other technologies that connect and exchange data with other devices and systems over the Internet or other communication networks.

### IoT Systems Management

- **Device Management:** ensure secure data transmission to facilitate fine interaction between devices and to guarantee the proper functioning of devices in an IoT system
- **User Management:** provide control over the users who have access to an IoT system. User management includes identifying users, setting user roles and access levels, controlling access, etc.
- **Security Monitoring:** to address security breaches at early stages and to prevent malicious attacks on an IoT system, perform the activities such as log and analyze commands sent by control applications to things, monitor and store all

### IoT Security Best Practice

1. Disable the “guest” and “demo” user accounts if enabled
2. Use the “Lock Out” feature to lock out accounts for excessive invalid login attempts
3. Implement strong authentication mechanisms
4. Locate control system networks and devices behind firewalls and isolate them from the business network
5. Implement IPS and IDS in the network
6. Implement end-to-end encryption and use Public Key Infrastructure (PKI)
7. Use VPN architecture for secure communication
8. Deploy security as a unified, integrated system

### OT (Operational Technology)

[TechTarget: What is OT (Operational Technology)?](https://www.techtarget.com/whatis/definition/operational-technology)

> A category of hardware and software that monitors and controls how physical devices perform.

#### Why OT is important

> OT is critical for businesses and society at large.
> For example, in May 2021, a ransomware attack caused the Colonial Pipeline to be shut down.
> The pipeline, which itself is considered an OT, transports 2.5 million barrels of fuel each day.
> The shutdown resulted in a major East Coast fuel shortage.

#### Examples of OT environments

- Factories
- Power plants
- Oil and gas refineries and pipelines
- Transportation and aviation facilities
- Water treatment facilities

#### Examples of OT systems

- Robots
- Medical devices
- Distributed control systems
- ICS
- Industrial internet of things
- Programmable logic controllers
- Remote terminal units
- Smart buildings
- Smart transportation

#### Challenges of OT

- Lack of visibility
- Plain-text passwords
- Network complexity
- Legacy technology
- Lack of anti-virus protection
- Lack of skilled security professionals
- Rapid pace of change
- Outdated systems
- Haphazard modernization
- Convergence with IT
- Unique production networks / Proprietary software
- Vulnerable communication protocols

#### Industrial Internet of Things (IIOT)

Also known as OT/IT convergence. It uses the strength of both OT and IT for improved security.

#### Security Solutions

Firewalls:

- Firewalls are used in the network for monitoring and controlling the incoming and outgoing network traffic.
- You can use firewall solutions such as SCADAWall and Waterfall for securing the OT network.

Unified Identity and OT Access Management:

- Access management helps industries to centralize certain operations like adding, securing, changing, and removing
user access to the OT systems.
- You can use tools such as OTAccess and FireEye for identifying and managing access to industrial systems.

Asset Inventory and Device Authorization:

- Asset inventory helps in connecting only authorized devices to the network and detect vulnerabilities in the devices.
- You can use tools such as SCADAfence and CyberLens for asset inventory and device authorization.

OT Network Monitoring and Anomaly Detection:

- OT network monitoring employs machine learning algorithms for easy detection and identification of malicious
behaviors.
- You can use tools such as Claroty and OT ThreatFeed for OT network monitoring and anomaly detection.

Decoys to Deceive Attackers:

- Decoys are honeypots used in OT environments to lure attackers to reveal their presence and activities.
- You can use decoy tools such as ThreatDefend, Conpot, and GasPot for protecting the network.

### Guidance & NIS2 Directive

• [NIS Compliance Guidelines for Operators of Essential Service (OES)](https://ncsc.gov.ie/pdfs/NIS_Compliance_Security_Guidelines_for_OES.pdf)
• [NCSC: NIS2](https://ncsc.gov.ie/nis2/)

### The NIS2 Directive: What you need to know (video)

[NCSC: NIS2 videos](https://www.ncsc.gov.ie/nis2/videos/)

The video answer the 3 top FAQ about the NIS2 directive:

1. Am I in scope?
2. How do I comply?
3. How do I report incidents, and what can I expect?
