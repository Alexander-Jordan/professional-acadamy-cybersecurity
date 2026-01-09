# Unit 7: Introduction To Ethical Hacking

## Summary

- What is Ethical Hacking & Pen Testing?
- Steps in Planning a Penetration Testing
- Stages in Penetration Testing
- Ethical Hacking Tools & Demo

## U7P1: Unit Introduction

Learning outcomes:

- What is Ethical Hacking & Pen Testing?
- Steps in Planning a Penetration Testing
- Stages in Penetration Testing
- Ethical Hacking Tools & Demo
- [Ethical Hacking Whitepaper](https://pecb.com/en/whitepaper/ethical-hacking-whitepaper)

## U8P2: What is EH?

Uses the same tools as a normal hacker, but with permissions, to find weak points.

The exploitation of an IT system with the permission of its owner to determine its vulnerabilities and weak points. It is an effective way of testing and validating an organization’s cyber security position.

The results of ethical hacking are typically used to recommend preventive and corrective countermeasures that mitigate the risk of a cyber-attack.

### Why?

> To beat a hacker, you need to think like a hacker.

- To prevent hackers from gaining access to the organization’s information systems
- To uncover vulnerabilities in systems and explore their potential as a security risk
- To analyze and strengthen an organization’s security posture
- To provide adequate preventive measures to avoid security breaches
- To help safeguard customer data
- To enhance security awareness at all levels in a business

### Answers These Questions

- What can an intruder see on the target system? (Reconnaissance and Scanning phases)
- What can an intruder do with that information? (Gaining Access and Maintaining Access phases)
- Does anyone at the target organization notice the intruders’ attempts or successes? (Reconnaissance and Covering Tracks phases)
- Are all components of the information system adequately protected, updated, and patched?
- How much time, effort, and money are required to obtain adequate protection?
- Are the information security measures in compliance with legal and industry standards?

### Scope and Limitations

Scope:

Ethical hacking is a crucial component of risk assessment, auditing, counter fraud, and information systems security best practices
It is used to identify risks and highlight remedial actions. It also reduces ICT costs by resolving vulnerabilities

Limitations:

An ethical hacker can only help the organization to better understand its security system; it’s up to the organization to place the right safeguards on the network

### Technical Skills

- In-depth knowledge of major operating environments such as Windows, Unix, Linux, and Mac
- In-depth knowledge of networking concepts, technologies, and related hardware and software
- Knowledgeable about security areas and related issues
- Highly technical knowledge for launching sophisticated attacks

### Non-Technical Skills

- The ability to learn and adopt new technologies quickly
- Strong work ethics and good problem solving and communication skills
- Committed to the organization’s security policies
- An awareness of local standards and law

## U8P3: What is Pen Testing?

A type of security testing that evaluates an organization’s ability to protect its infrastructure such as network, applications, systems, and users against external as well as internal threats

It involves the active evaluation of the security of the organization’s infrastructure by simulating an attack similar to those performed by real attackers

### Benefits

- Reveal vulnerabilities
- Show real risks
- Ensure business continuity
- Reduce client-end attacks
- Establish the status of a company in terms of security posture
- Protect the reputation of the organization
- Meet compliance obligations

### Prerequisites

- Planning and Scoping
- Target audience
- ROE (Rules of Engagement)
- Communication Escalation Path
- Resources
- Budget
- Impact & Disclaimers
- Constraints

### Contracts

- SOW (Statement of Work)
  - Clearly states what tasks are to be accomplished during an engagement
- MSA (Master Service Agreement)
  - High level contract between a service provider and a client that specifies details of the business arrangement
- NDA (Non‐Disclosure Agreement)
  - Agreement that defines confidential material and restrictions on use and sharing sensitive information with other parties
- WRITTEN AUTHORIZATION
  - Obtain signature from proper signing authority
    - “Get out of jail free” card
    - Pen tests can reveal sensitive or confidential information
    - Activities may be illegal without proper permission
    - Signed permission makes you a white hat pen tester
  - Third‐party authorization when necessary
    - Ex: from a Cloud service provider Get permission for any outside resources used
      - Cloud, Internet (ISP usage), etc

### Understanding the Target Audience

Characteristics of your target audience:

- Need for the report
- Position of the primary recipient
- Main purpose and goal of the test and the report
- Individual or business unit responsibility and authority to make decisions based on the findings
- Who the report will be addressed to
- Who will have access to the report

### The Law

ICLG.com Cybercrime & Irish Law:  

> Hacking (i.e. unauthorized access) is an offense under section 2 of the Criminal Justice (Offenses Relating to Information Systems) Act 2017 (the ”2017 Act”).
> A person who, without lawful authority or reasonable excuse, intentionally accesses an information system by infringing a security measure, commits an offense.

### Rules of the Engagement

- Define the conditions under which the test will be conducted
- Document and agree upon these rule of engagement conditions with the client or an appropriate stakeholder
- Permission to test document

### Types of tests

#### Security Audit

A security audit checks whether an organization follows a set of standard security policies and procedures

#### Vulnerability Assessment

A vulnerability assessment focuses on discovering the vulnerabilities in an information system, but provides no indication whether the vulnerabilities can be exploited or the amount of damage that may result from the successful exploitation of the vulnerabilities

#### Penetration Testing

Penetration testing is a methodological approach to security assessment that encompasses a security audit and vulnerability assessment, and it demonstrates whether the vulnerabilities in a system can be successfully exploited by attackers

### Steps for Planning a Penetration Test

1. Understand the environment
2. Set test objectives
3. Define the test scope
4. Assess the risks
5. Define the methodology
6. Ensure management approval
7. Decide who is going to conduct the tests and when
8. Allocate the resources
9. Inform the IT team
10. Define what the report should include

### Penetration Testing Methodologies

- Web application tests
- Network infrastructure tests
- Wireless network tests
- Physical facility tests
- Social engineering tests

 Others:

- PTES (Penetration Testing Execution Standards)
- PCI DSS penetration testing guidance
- Penetration Testing Framework
- NIST Special Publication 800-115
- OSSTMM (Open Source Security Testing Methodology Manual)
- OWASP Testing Project

### Penetration Testing Strategies

#### Black-box test (aka zero-knowledge testing)

Simulates the actions and procedures of a malicious attacker who has no prior knowledge about the target.
Black box testing is further classified into blind testing and double-blind testing.

#### White-box test (aka complete-knowledge testing)

Simulates the actions and procedures of an attacker who has prior knowledge on the target.
It provides a much more cost-effective way to quickly reveal misconfigurations and vulnerabilities, as well as assuring complete testing coverage.

#### Gray-box test (aka partial-knowledge testing)

Combines the methodologies of both black box and white box testing.
It consists of a methodical attack that simulates testing with limited information on
the target.

### Activity: Planning a pen test

[Penetration Testing Execution Standard](http://www.pentest-standard.org/index.php/Main_Page)

Defines seven sections of a penetration test:

1. Pre‐engagement interactions
2. Intelligence Gathering
3. Threat Modelling
4. Vulnerability Analysis
5. Exploitation
6. Post Exploitation
7. Reporting

Take 15 mins to review the Penetration Testing Execution Standard

## U8P4: Phases

- Information gathering
- Scanning and enumeration
- Gaining access
- Maintaining access
- Clean up
- Reporting

### Challenges

- [Try Hack Me](https://tryhackme.com/room/pentestingfundamentals)
- [picoCTF](https://picoctf.org/)

### Activity: Try Hack Me

- Register for a free account with Try Hack Me
- Follow this link and compete the Pen Testing Fundamentals room
- [Try Hack Me](https://tryhackme.com/room/pentestingfundamentals)
- Optional: Choose another room to complete.

## U8P5-6: OSINT

- Gathering publicly available intelligence resources to collect and analyze information about a target
- Does not require any type of covert methods
- Most information can be found on the Internet
- Recon-ng
- Shodan

## U8P7-8: Lazarus Heist (video)

[How North Korean Hacking Actually Works | The WannaCry Attack](https://www.youtube.com/watch?v=UsoQTKXt_Wk)

## U8P8-9: Frameworks

### Exploitation Frameworks

- Metasploit
  - auxiliary
  - encoders
  - exploits
  - nops
  - payloads
  - post (for post-exploitation)
- BeEF

### Bash Shell

- Command shell and language interpreter
- Available for Linux, Mac OS X, and even Windows
- Being familiar with bash enables you to create scripts, parse data, and automate tasks
- [Linux Config bash scripting tutorial](https://linuxconfig.org/bash-scripting-tutorial)
- [DevHints bash shell programming cheat sheet](https://devhints.io/bash)

### Python

- Popular programming language
- Can be used to automate repetitive tasks and create applications
- [W3 Schools Python Tutorial](https://www.w3schools.com/python)
- [Tutorials Point Python Tutorial](https://www.tutorialspoint.com/python/index.htm)
- [The Python Guru](http://thepythonguru.com)
- [A comprehensive list of Python resources](https://github.com/vinta/awesome-python)

### Books & Resources

- [Hack the box](https://www.hackthebox.eu/)
- TCM Academy: Ethical Hacking in 15 Hours - Free
- [Try hack me](https://tryhackme.com/)
- Ecollege.ie: CompTIA PenTest+
- [Scholarship: not free](https://fortifyinstitute.eccouncil.org/)

#### YouTube channels

- [John Hammond](https://www.youtube.com/@_JohnHammond)
- [Rana Khalil](https://www.youtube.com/@RanaKhalil101)
- [Chris Greer](https://www.youtube.com/@ChrisGreer)
- [The Cyber Mentor](https://www.youtube.com/@TCMSecurityAcademy)

### Certifications

- CEH (Certified Ethical Hacker)
- CCT (Certified Cybersecurity Technician)
- CompTIA PenTest+
- PJPT & PNPT

## U8P10-11: Pen Test report

- Report should be detailed and specific
  - Customers will need to make changes based on the findings
  - Customer should feel they got value for money
- Results should be validated
- Avoid reporting false positives
  - May cause a loss of customer confidence

### Common Report Elements

- Executive summary
  - Goals & general findings
- Methodology
  - Approach taken
  - Tools and techniques
  - Assumptions
- Findings and remediation
  - Ranked list
    - What you found listed by priority
    - What you recommend the client does provide options as
- Metrics and measures
  - Details of findings
  - Risk Rating
- Conclusion
  - Wrap up, summary, CTA (Call To Action)

### Samples & Templates

- [PTES: Reporting](http://www.pentest-standard.org/index.php/Reporting)
- [GitHub: juliocesarfort/public-pentesting-reports](https://github.com/juliocesarfort/public-pentesting-reports)

### Report Best Practice

- Risk appetite
  - Amount of risk client is willing to accept
  - Tone of the entire report is based on the company’s appetite for risk
  - Risk appetite statement should appear in the report introduction
- Report storage
  - Reports should become part of the organization’s document repository
  - Used as input for future pen tests and other assessments
  - Security policy should state how long reports are kept
- Report handling and disposition
  - Security policy should state how assessment reports are stored
  - At end of life, how are reports disposed of?

### Post-Engagement Activities

- Remove any malicious scripts
- Clean any information added to databases
  - Restoring database to a previous state is best
- Remove any user accounts created
- Clean up any files left from successful or unsuccessful exploitation attempts
- Have the client or system owner validate that the cleanup is sufficient
- Client acceptance
  - Formal cessation of project activities and acceptance of deliverable
  - Client should sign a statement of acceptance
- Lessons learned
  - Crucial step in project closure
- Follow-up actions/retest
  - Client may need more actions based on findings
  - Be careful to avoid extending the project scope here without a change process
- Attestation of findings
  - Independent review and assurance of findings (i.e. third party)

### Recommended Mitigation Strategies

- Nearly every pen test will discover multiple vulnerabilities
- A pen test report should contain recommendations to mitigate each vulnerability
- Solutions vary, depending on the vulnerability
- **People**–behavior changes
  - Social engineering
  - Passwords
- **Process** how things are done
  - Backup media handling
  - ID management
- **Technology**
  - Controls based on hardware and/or software

### Common Findings

- Shared local administrator credentials
  - Randomize credentials/LAPS
- Weak password complexity
  - Minimum password requirements/password filters
- Plain text passwords
  - Encrypt the passwords
- No multi-factor authentication
  - Implement multi-factor authentication
- SQL injection
  - Sanitize user input/parameterize queries
- Unnecessary open services
  - Disable or remove unneeded services (system hardening)

### Video

[If You Want to Be a Pen Tester, You MUST Watch This!](https://www.youtube.com/watch?v=1MSHX4ynD4U)
