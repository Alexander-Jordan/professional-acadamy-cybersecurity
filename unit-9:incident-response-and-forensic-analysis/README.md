# Unit 7: Incident Response & Forensic Analysis

## Summary

- Incident Response
- Digital Forensics
- ACPO Principles
- Practical Demonstration

## U9P1: Unit Introduction

Learning outcomes:

- Incident Response
- Digital Forensics
- ACPO Principles
- Practical Demonstration

## U9P2: Incident Response

The process of taking organized and careful steps when reacting to a security incident.

Involves a sequence of steps that begin with first identifying and reporting an incident.

Processes differ from organization to organization according to their business and operating environment.

The IH&R (Incident Handling and Response) team is a group of specialized people who collectively respond, remediate, mitigate, recover, and communicate the impact of incidents.

The IH&R team works on an incident response plan when dealing with a security incident.

### Roles & Responsibilities of IH&R Team

- Management
- Information Security Team
- IT Staff
- Physical Security Staff Legal
- HR Representative
- PR/Comms
- Financial Auditor
- IR Officer
- IR Manager
- IR Assessment Team

### First Responder

An individual who arrives first at the incident scene and brings the incident to the attention of others.

Could be an end user, network administrator, or any other individual who is involved in the day-to-day network operations.

Plays a key role in incident response and forensic investigation process.
They can provide great help in early detection of incident, source of the incident, impact of incident, evidence collection and preservation, etc.

### First Responder Tasks

- **Reporting** the incident
- **Containing** incident
- **Alerting** the management and incidence response teams
- **Identifying** the crime scene
- **Collecting** the complete information about the incident
- **Documenting** all the findings
- **Protecting** the crime scene
- **Preserving** temporary and fragile evidence
- **Packaging** and transporting the electronic evidence

### Purpose of IH&R

- Protect networks and systems
- Ensure timely incidents handling
- Ensure the gathering of appropriate information
- Identify false positives
- Efficiently use resources
- Address legal issues
- Comply with local, national, and international guidelines
- Train and protect personnel
- Develop comprehensive documentation

### Incident Response Plan

- Address the mission and vision statements
- Meet the goals of incident response initiative
- Comply with the statement of senior management approval
- Include strategies to achieve set goals and timelines
- Have an organized approach to incident response
- Identify incident response key performance indicators that organization can use for future reference
- Provide a statement of interoperability
- Add value to other organizational processes
- Make efficient use of all the resources
- Strengthen the organization’s security

## U9P3: Digital Forensics and ACPO Principles

What is Digital Forensics?

NIST:

> Digital forensics is the field of forensic science that is concerned with retrieving, storing and analyzing electronic data that can be useful in criminal investigations. This includes information from computers, hard drives, mobile phones and other data storage devices.

EC-Council:

> Computer forensics refer to a set of methodological procedures and techniques that help identify, gather, preserve, extract, interpret, document, and present evidence from computing equipment, such that any discovered evidence is acceptable during a legal and/or administrative proceeding

### History of Digital Forensics

- 1970s evolved with cyber crime
- 1984 FBI formed the CART (Computer Analysis Response Team)
- 2004 EU established a treaty on Convention on Cybercrime
- 2005 ISO published a standard ISO 17025

### Objective of CF

- **Identify**, gather, and preserve the evidence of a cybercrime
- **Minimise** the tangible and intangible losses to the organization
- **Gather** evidence of cybercrimes in a forensically sound manner
- **Protect** the organization from similar incidents in the future
- **Estimate** the potential impact of malicious activity on the victim and assess the intent of the perpetrator
- **Support** the prosecution of the perpetrator of an incident

### What is Digital Evidence?

> Any information of probative value that is either stored or transmitted in a digital form

Circumstantial and fragile in nature, which makes it difficult for a forensic investigator to trace criminal activities

According to Locard's Exchange Principle:

> Anyone or anything, entering a crime scene takes something of the scene with them, and leaves something of themselves behind when they leave.

### eDiscovery

Same process as Digital Forensics, however output is processed in a legally admissible manner by a suitable qualified professional.
Specialized software and embedded in popular applications.

Digital Forensics:
Who, what, where, when, why & how?
Seizure (identifying what to take as evidence), Acquisition (creating a copy of the evidence for analysis), Analysis, Report.

### EDRM (Electronic Discovery Reference Model)

[EDRM PDF](https://edrm.net/wp-content/uploads/2020/04/EDRM-clean-poster-24x36-1.pdf)

### Rules of Evidence

- **Understandable**: Evidence must be clear and understandable
- **Admissible**: Evidence must be related to the fact being proved
- **Authentic**: Evidence must be real and appropriately related to the incident
- **Reliable**: There must be no doubt about the authenticity or veracity of the evidence
- **Complete**: The evidence must prove the attacker’s actions or his/her innocence

### Types of Digital Evidence

#### Volatile Data

Data that are lost as soon as the device is powered off; examples include system time, logged-on user(s), open files, network information, process information, process-to-port mapping, process memory, clipboard contents, service/driver information, command history, etc.

#### Non-volatile Data

Permanent data stored on secondary storage devices such as hard disks and memory cards; examples include hidden files, slack space, swap file, index.dat files, unallocated clusters, unused partitions, hidden partitions, registry settings, event logs, etc.

### Roles of Digital Evidence

- Identity theft Malicious attacks on the computer systems Information leakage
- Unauthorized transmission of information
- Use/abuse of the Internet
- Theft of commercial secrets
- Production of false documents and accounts
- Unauthorized encryption/ password protection of documents
- Abuse of systems
- Email communication between suspects/conspirators

### Sources of Potential Evidence

#### User-Created Files

- Address books
- Database files
- Media (images, graphics, audio, video, etc.) files
- Documents (text, spreadsheet, presentation, etc.) files
- Internet bookmarks, favorites, etc.

#### User-Protected Files

- Compressed files
- Misnamed files
- Encrypted files
- Password-protected files
- Hidden files
- Steganography

#### Computer-Created Files

- Backup files
- Log files
- Configuration files
- Printer spool files
- Cookies 
- Swap files
- System files
- History files
- Temporary files

### ACPO Principles

1. **Evidence should not be changed**: No action taken by law enforcement agencies, persons employed within those agencies, or their agents should change data which may subsequently be relied upon in court.
2. **Competence to access original data**: In circumstances where a person finds it necessary to access original data, that person must be competent to do so and be able to give evidence explaining the relevance and the implications of their actions.
3. **Keep a detailed log of actions**: An audit trail or other record of all processes applied to digital evidence should be created and preserved. An independent third party should be able to examine those processes and achieve the same result.
4. **Somebody has to be accountable**: The person in charge of the investigation has overall responsibility for ensuring that the law and these principles are adhered to.

### Scenario One

- You attend a police raid and a suspect has been arrested
- You have been told to gather electronic evidence
- You enter a room and a PC is currently turned on and logged in

What do you do?

#### Choices

1. Close all applications and shutdown the machine using the correct OS shutdown procedure
2. Unplug the power cable from the PC
3. Press and hold the power button until the PC turns off

What do you do?

#### Answer

Choice number 2: Unplug the power cable from the PC

Why?
The following changes occur when shutting down or logging of a machine:

- Flush the cache to disk
- Write to a log file
- (Potentially) Initialize OS updates/upgrades

All of these actions count as altering evidence and can result in said evidence becoming inadmissible.

It is very important to unplug the power cable from the PC!
This also avoids any data being written to the hard drive if an uninterruptible power supply is fitted.

It is also very important that you do not close any applications as this may also cause data to be written to the hard drive

Why not press and hold the power button?
On some PCs, pressing the power button may initiate a “sleep” or “log off” procedure, which will trigger some OS actions and alter data on the hard disk.

> [!NOTE]  
> A lot of laptops are being used nowadays, and the recommended procedure used to be to unplug the battery.
> But in a lot of laptops today it's simply not possible.

### Roles & Responsibilities of Forensic Investigator

- Determines the extent of any damage done during the crime
- Recovers data of investigative value from computing devices involved in crimes
- Creates an image of the original evidence without tampering with it to maintain its integrity
- Guides the officials carrying out the investigation
- Analyses the evidence data found
- Prepares the analysis report
- Updates the organization about various attack methods and data recovery techniques, and maintains a record of them
- Addresses the issue in a court of law and attempts to win the case by testifying in court

### Phases in Forensic Investigation

#### Pre-investigation Phase

Involves setting up a computer forensics lab, building a forensics workstation, developing an investigation toolkit, setting up an investigation team, getting approval from the relevant authority, etc.

#### Investigation Phase

Involves acquisition, preservation, and analysis of evidentiary data to identify the source of the crime and the culprit behind it.

#### Post-investigation Phase

Ensures that the report is easily explicable to the target audience and that it provides adequate and acceptable evidence.

### Digital Forensic Investigation

- Seizure (identifying what to take as evidence)
- Acquisition (creating a copy of the evidence for analysis)
- Analysis
- Reporting

### Seizure

- Control the ‘crime’ scene
- Identify relevant evidence
- Preserve the evidence
- Restrict access
- Document everything
- Do not power off! (unless having it on removes the data or doing other harm)
- Comprehensive photos, film & notes of location, peripherals, etc.
- Tag, label & inventory.
- Anti-static bags
- Evidence bags
- Faraday bags (for mobile devices)

## U9P4: Powered On

- **Photograph**: If a computer is switched ON and the screen is viewable, photograph the screen and document the running programs
- **Record**: If a portable computer wakes up, record the time and date at which this occurs, take a photograph of the screen, and document a brief explanation of all running programs
- **Move**: If a computer is ON and the monitor shows a screensaver, move the mouse slowly without pressing any mouse button and then photograph and document the programs
- **Turn off**: After collecting all volatile data, turn off the devices
- **Press down**: For portable computers, press down the power switch for 30 seconds to force the power off
- **Remove**: For portable computers, remove the battery and unplug the power cord from the wall socket
- **Leave**: If the computer is switched OFF, leave it in that state

### Chain of Custody

> How evidence is collected, transported & presented at every stage.
> Full lifecycle from collection to return/destruction.

### Acquisition

> Extracting digital contents so they may be analyzed.

Analysis carried out on verified copy of evidence.

- **Prepare** the destination media
- **Prevent** changes to the original.
- **Hash** the original evidence (and then the copy as well).
- **Copy** the evidence (bit by bit, even the deleted or allocated space).
- **Verify** the acquisition.
- **Safeguard** the original evidence.

### Write Blocker

[Wikipedia: Forensic disk controller](https://en.wikipedia.org/wiki/Forensic_disk_controller):

> A specialized type of computer hard disk controller made for the purpose of gaining read-only access to computer hard drives without the risk of damaging the drive's contents.

### Analysis – Log Files

#### Network Logs

Record events related to system or user activities such as accessing a resource, performing authentication, and details of communication with remote hosts that contain critical information such as IP addresses, date, timestamp, details of request, and response messages.

#### System Logs (syslog)

Provide details of process success state, devices, warnings, system failures, debugs, errors, and alerts, etc. that contain critical information for investigating an incident.

#### Application Logs

Records all events or actions generated during the runtime of an application.

These records can be investigated to identify the behavior of server and details of entities (who, when, and how) accessing the serve.

### Reporting

Needs to be ...

- Comprehensive
- Facts stated
- Assumptions stated
- Generated with audience in mind
- May be generated by software suite

### DF software suites

Can do ...

- Acquisition
- Analysis
- Reporting

Software examples:

- EnCase
- FTK (Forensic Toolkit)
- The Sleuth Kit: Autopsy (GUI)

### Activity: Browser forensic

In your browser, type in the URL section ...

- On Chrome: chrome://about
- On Firefox: about:about

Now browse around the different options like logs, history, or configs.

## U9P5: Mobile Forensics

- Require specialist software
- Variety of cables
- Once in, most data retained.
- Much data on cloud, SIM & service provider.
- Eg. Oxygen Forensics Detective

### Digital Forensic Kit

- Jump Bag
- Laptop
- Write Blockers and Drive Adapters
- Cables
- Wiped Removable Media
- Camera
- Tamper-Proof Seals
- Forms
  - Chain of Custody Form
  - Incident Response Plan
  - Incident Log
  - Call/Escalation List

### Challenges

- More devices
- Larger storage
- Encryption
- Data in cloud
- Evading detection
  - Steganography
  - Time stomping
  - Changing file ext
  - Bit shifting

## U9P8: Resources

Books:

- Guide to computer forensics and investigations, by Bill Nelson, Amelia Phillips, Christopher Steuart
- A practical guide to computer forensics investigations, by Dr. Darren R. Hayes

### Activity: THM digital forensics

[TryHackMe: Intro digital forensic](https://tryhackme.com/r/room/introdigitalforensics)

## U9P10: References

- [Microsoft Advanced eDiscovery](https://docs.microsoft.com/en-us/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide)
- [Build a Digital Forensics Lab on a Budget](https://bhconsulting.ie/how-to-build-your-first-digital-forensics-lab-on-a-budget/)

Standards & Frameworks:

- European Network of Forensic Science Institutes (ENFSI)
- NIST publications
- ISO standards
- Digital Evidence (SWGDE)
- SANS Institute community resources

- [Top 10 Free Tools for DF Investigation](https://www.qa.com/about-qa/our-thinking/top-10-free-tools-for-digital-forensic-investigation/)
- [E discovery Guidebook](https://www.algoodbody.com/media/Pentest-mag-ediscovery-article1.pdf)
- [How Facebook works with Law Enforcement](https://www.facebook.com/safety/groups/law/guidelines/)
