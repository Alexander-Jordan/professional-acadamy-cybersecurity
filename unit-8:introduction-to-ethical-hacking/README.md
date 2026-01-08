# Unit 7: Introduction To Ethical Hacking

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
