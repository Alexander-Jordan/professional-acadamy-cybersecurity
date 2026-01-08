# Unit 7: Risk Management, BC & DR

## Summary

- Risk Management
- Types of Risks
- Risk Management Frameworks
- Business Continuity & Disaster Recovery Overview
- BC/DR Plans

## U7P1: Unit Introduction

Learning outcomes:

- Risk Management
- Types of Risks
- Risk Management Frameworks
- Business Continuity & Disaster Recovery Overview
- BC/DR Plans

## U7P2: Risk Management

> NIST definition:
> The process of identifying, assessing, and taking steps to reduce risks to an acceptable level.
> This involves conducting risk assessments to determine the extent of potential threats and vulnerabilities, followed by implementing appropriate controls to mitigate identified risks.
> The process also includes continuous monitoring of the security state of the information systems to ensure that risks remain at an acceptable level.

### Benefits

- Focuses on potential risk impact areas
- Addresses risks according to the risk level
- Improves the risk handling process
- Allows the security officers to act effectively in adverse situations
- Enables effective use of risk handling resources
- Minimizes the effect of risk on the organization’s revenue
- Identifies suitable controls for security

### Definitions

- **Risk management:** coordinated activities to direct and control an organization with regard to risk
- **Risk assessment:** overall process of risk identification, risk analysis and risk evaluation
- **Risk identification:** assets, threats, vulnerabilities, current controls, consequences
- **Risk analysis:** process to comprehend the nature of risk and to determine the level of risk
- **Risk evaluation:** process of comparing the results of risk analysis with risk criteria to determine whether the risk and/or its magnitude is acceptable or tolerable (you can't remove risk entirely)
- **Risk treatment:** process of selection and implementation of measures to modify risk
- **Risk acceptance:** decision to accept a risk
- **Residual risk:** the risk remaining after risk treatment

### Key Roles/Responsibilities

- Senior Management
- CIO (Chief Information Officer)
- System and Information Owners
- Business and Functional Managers
- IT Security Program Managers
- IT Security Practitioners
- Security Awareness Trainers

### Key Risk Indicators

[TechTarget: What is a key risk indicator (KRI) and why is it important?](https://www.techtarget.com/searchcio/definition/key-risk-indicator-KRI)

> KRI (Key Risk Indicator) is a metric for measuring the likelihood that the combined probability of an event and its consequences will exceed the organization's risk appetite and have a profoundly negative impact on an organization's ability to be successful.
> Risk appetite is the amount of risk an organization or investor is willing to take in pursuit of objectives it deems have value.

#### Creating measurable KRIs

1. **Define objectives:** Identify the business attributes that are important to the organization and the objectives it wants to achieve with KRIs.
2. **Identify risks:** Articulate all risks the organization faces, including financial, operational, compliance and cybersecurity risks.
3. **Connect risks and objectives:** Show how each risk could affect the organization's ability to achieve its objectives. Rank risks in terms of their importance in achieving objectives.
4. **Define KRIs:** Based on previous steps, develop measurable KRIs to monitor and measure whether the identified risks are materializing.
5. **Get approvals:** Secure senior management approval of KRIs.
6. **Set thresholds:** Establish measurable levels for each KRI that indicate when risk becomes unacceptable and to trigger a response.
7. **Find data sources:** Identify the data needed for measuring the KRI and how it will be collected. This could include financial reports, operational metrics and incident reports.
8. **Establish measurement systems:** Put in place systems, processes and tools to regularly measure the KRIs.
9. **Monitor and evaluate:** Continuously monitor the KRIs to track the changes in risk levels, assess KRI effectiveness and take necessary action.
10. **Reporting:** Summarize and communicate KRI data and insights into the risk levels to relevant stakeholders and decision-makers.
11. **Review and improve:** Regularly assess KRI effectiveness at capturing risks, and revise them as needed.

#### Examples

- Loss of staff: An organization's business can be negatively affected when employees are sick, are disabled, leave for another job or retire. It's important to have KRIs in place monitoring employee absenteeism to identify when it exceeds a critical level. For example, this type of KRI measurement might have a threshold of a 20% decline in total head count.
- IT disruptions. A KRI should identify the optimum patch level for cybersecurity systems. The threshold level might be something like, when the cybersecurity system patching is two patches behind the scheduled and recommended levels, the KRI kicks in.
- Failed backup. When backup systems fail, it can be difficult to recover systems, data files and databases to the current state. A KRI should be created to monitor that IT assets are at their most current backup levels. It might be set to send an alert when backup levels fall below minimum acceptable time frames.

> [!IMPORTANT]  
> It isn't enough to simply create KRIs and walk away.
> Good risk management requires they be regularly monitored and reviewed to identify situational changes that indicate a change in the business.
> They also must be monitored for changes in risk and threat levels and to identify and initiate remedial action that may be needed.

### Types of Risk

- Risks from Internal Sources
- Risks from External Sources
- Intellectual Property Theft
- Risk from Legacy Systems
- Multi-Party Risks
- Software Compliance Risks

### Risk Management Phases

#### Identification of Key business assets

- Identify key business process, supporting application, and supporting application
- Assign an asset value

#### Risk Identification

- Identify threats, vulnerabilities, impact, and existing controls

#### Risk Analysis

- Assess impact, likelihood, and risk level

#### Risk Evaluation

- Evaluation of risk based on risk evaluation criteria

#### Risk Treatment

- Risk treatment options and plan
- Evaluation of residual risk

#### Risk Acceptance

- Risk treatment plan/Acceptance plan
- Residual risk acceptance

### Risk Definitions

- **Asset:** Anything of value (including brand and reputation)
- **Threat:** Negative impact to asset
- **Threat Agent:** What carries out attack
- **Vulnerability:** Weakness
- **Exploit:** IOC (Instance of Compromise)
- **Risk:** Probability of a threat exploiting a vulnerability
- **Controls:** Physical, Administrative, Technical
  - **Safeguards:** Deterrents or Preventatives
  - **Countermeasure:** Detective or Corrective
- **Total Risk:** Before control implemented
- **Residual Risk:** After applying control
- **Secondary Risk:** One risk response triggers another event

## U7P3-4: What is Risk?

> NIST:  
> Risk is the potential for an unwanted outcome resulting from an event, as determined by its likelihood and the impact of the event. It is the possibility that a threat will exploit a vulnerability to cause harm to an organization or individual.

Risk is what we try to minimize.

### Identification

Establishing context:

- Understand the current posture the organization operates in
- Define the external and internal environment in which the organization operates

Quantifying risks:

- Determines the effect of the risk
- Calibrates the possible outcome of risks

### Risk assessment

- Assesses the organization's risk and provides an estimate on the likelihood and impact of the risk
- On-going iterative process, assigning priorities, and implementation plans
- Determines the quantitative (numbers) and qualitative (words) value of risk

### Risk Analysis: Quantitative (Numbers)

Mapping the probability of a specific event occurring to the perceived cost of the event

### Quantitative Assessment

#### Likelihood

- ARO (Annual Rate of Occurrence): event number / years
- If a flood occurs every 10 years, the ARO is 10%

#### Exposure

- EF (Exposure Factor): SLE / AV (Assets Value)
- Facility’s AV is $20 million, expected loss is $4 million in a flood
- EF is 20%.

#### Impact

- SLE (Single Loss Expectancy): EF * AV (Assets Value)
- Flooding incurs 20% EF, the facility’s value is $20 million
- SLE is $4 million

#### Risk

- ALE (Annual Loss Expectancy) = ARO * SLE
- Flood occurs once every 10 years, expected loss is $4 million for
each flood
- ALE is $400,000

### Activity 1

> The asset value of a small office building and its contents is €2 million.
> This building houses the call centre and the complete loss of the centre would take away half of the capability of the company.
> A fire at this business’s location is expected to occur about once in 20 years.
> What is the SLE?
> And from that, what is the ALE?

Answers:

- EF: 50%
- SLE: €1 million
- ARO: 5%
- ALE: €50 000

## U7P5: Risk Analysis

### Qualitative (Words)

- Focuses on mapping the perceived impact of a specific event occurring to a risk rating agreed upon by the organization.
- Most methodologies use interrelated elements such as threats, vulnerabilities, and controls

An example could be if you are an influencer with a lot of followers. If you'd be hacked and it lead to you loosing all your followers, how much would it cost you to recover that type of following? That's how qualitative risk analysis comes in.

### Assessment of Overall Impact

The final stage of risk identification is identification of the impacts on the organization that might be caused by an incident scenario.

Examples of consequence could be:

- Financial loss
- Loss of an asset or its value
- Loss of customer or supplier
- Prosecution or penalty
- Loss of privacy
- Service interruption
- Loss of reputation or brand damage
- Inability to meet contractual obligations
- Breach of security, staff or users

### Risk assessment matrix

[Industry risk: Risk assessment matrix](https://industryrisk.com.au/risk-assessment-matrix/)

### Risk Prioritization

- In order to identify the various risks with the same severity, the risks should be prioritized and rated
- While performing the risk response step, consider the risk prioritization
- The prioritization depends on the goals and resources of an organization

### Risk treatment

Process of selecting and implementing appropriate controls on the identified risks.

- Risks are addressed and treated based on its severity level
- Decisions made in this phase are based on the results of a risk assessment

### Responses to Risk

#### Avoidance

- When risk is likely, and impact is great.
- Computer equipment could be stolen if an office window is broken. Move equipment to an alternate location.

#### Mitigation

- When risk is likely, but impact is not excessive.
- Leave equipment in place, but add bars to the window.

#### Transfer

- When risk is unlikely, but impact is great.
- Offloading the responsibility to a third party, usually an insurance company.
- Leave equipment and window in place, but add insurance coverage.

#### Acceptance

- When risk is unlikely, and impact is minimal, or if cost outweighs benefit.
- Do nothing if theft is unlikely and equipment is not sensitive or valuable.

### Risk Categories

#### Inherent Risk

Risk that exists before controls are implemented.
Understand the potential risk impact that exists before controls are implemented to understand the value and effectiveness of the mitigation strategy.

#### Residual Risk

Residual risk is what remains after controls are implemented.
The most important consideration for residual risk is the understanding that some quantity of risk always remains after applying mitigation.

### Risk Treatment Plan

- Proposed security controls with priorities and deadlines
- Required resources
- Roles and responsibilities of stakeholders responsible for the proposed action
- Required performance
- Reporting and monitoring requirements

## U7P6: Control Types

- **Administrative**
  - Covers personnel security, risk management, training, permissions, etc.
  - Example: Security guards consult an access list to determine who is allowed access to the building without questioning.
- **Physical**
  - Limit a person’s physical access to assets or facilities, using locks, doors, fences, etc.
  - Example: Infrared monitoring system can detect the presence of an intruder.
- **Technical**
  - Implemented in computing environments like operating systems, applications, databases, network devices, etc.
  - Example: A user sign-in process requiring an account name and password for authentication to a network.

### Risk Tracking and Review

- **Risk Tracking**
  - The risk tracking phase identifies the chance of a new risk occurring
  - The tracking phase ensures appropriate controls are implemented to handle risks
  - Risk tracking also includes monitoring the probability, impact, status, and exposure of risk
- **Risk Review**
  - The review phase evaluates the performance of the implemented risk management strategies
  - Risk reporting ensures management is aware of the top risks, enabling them to plan to reduce the risk appropriately

[Wentz Wu: The NIST Generic Risk Model](https://wentzwu.com/2019/08/26/the-nist-generic-risk-model/)

### Risk Management Frameworks

Frameworks ensure risks are handled in the context of:

- The nature of the risks faced by the organization.
- The organization's risk tolerance.
- The resources available to manage risks.
- The organization's culture.

Common frameworks:

- ERM (Enterprise Risk Management) Framework
- ISACA Risk IT Framework
- ISO 31000, ISO 27005
- COSO Enterprise Risk Management Framework
- NIST 800 Risk Management Framework: works with NIST Cyber Security Framework

### Guidelines for Implementing Risk Management

- Construct program around process of analysis, prioritization, response, and monitoring and measuring.
- Integrate into a larger framework of GRC (Governance, Risk management, and Compliance).
- Follow phases of the risk analysis process.
- Identify all assets that are susceptible to risk.
- Place value on assets using one or more valuation methods.
- Identify how each asset is vulnerable.
- Identify threats to each vulnerable asset.
- Assess risk using qualitative or quantitative language.
- Prioritize risks.
- Respond to risk in different ways depending on the context.
- Select controls based on cost effectiveness, practicality, and efficacy.
- Consider residual risk as a way to review efficacy of your controls.
- Monitor and measure effectiveness of risk response techniques and management processes.
- Continuously improve the risk management program.

### Activity 2

#### Zero Trust Model

What is a zero-trust model?

[What is the zero-trust security model?](https://www.techtarget.com/searchsecurity/definition/zero-trust-model-zero-trust-network)

#### Assume Breach

What is Assume Breach Mentality?

[3 Ways to Implement an Assume Breach Mentality](https://cyberireland.ie/three-ways-implement-an-assume-breach-mentality/)

## U7P7: Game over Zeus (video)

[GameOverZeus - inside the hunt for the world's most powerful cyber-criminals](https://www.youtube.com/watch?v=7i3Iy98EAm8)

## U7P8-9: BC/DR

### What is BC (Business Continuity) & DR (Disaster Recovery)

- **BC** is a comprehensive approach to making sure you can keep making money.
- **DR** is the process by which you resume business after a disruptive event, (natural or man-made).

Often, the two terms are married under the acronym **BC/DR**. BC/DR determines how a company will keep functioning after a disruptive event until its normal facilities are restored.

### BCP/DRP (P: Plan) – How they differ

#### BCP

- Activities required to ensure the continuation of critical business processes
in an organization
- Alternate personnel, equipment, and facilities
- Often includes non-IT aspects of business
- Can contain COOP (Continuity of Operations Plan), Crisis Communications Plan, Critical Infrastructure Protection Plan, Cyber Incident Response Plan, DRP (Disaster Recovery Plan), ISCP (Information System Contingency Plan), Occupant Emergency Plan.

#### DRP

- Assessment, salvage, repair, and eventual restoration of damaged facilities and systems
- Often focuses on IT systems

### Industry Standards for BCP and DRP

- ISO 22301 specifies requirements to plan, establish, implement, operate, monitor, review, maintain and continually improve a documented management system to protect against, reduce the likelihood of occurrence, prepare for, respond to, and recover from disruptive incidents when they arise.
- ISO 27001 Requirements for Information Security Management Systems. Section 14 addresses business continuity management.
- ISO 27002 Code of Practice for Business Continuity Management.
- NIST 800-34
  - Contingency Planning Guide for Information Technology Systems. Seven step process for BCP and DRP projects
  - From U.S. National Institute for Standards and Technology

### What is a Business Continuity Plan?

SANS definition 1:

> BC (Business Continuity) refers to the activities required to keep your organization running during a period of displacement or interruption of normal operation.

DR (Disaster Recovery) is the process of rebuilding your operation or infrastructure after the disaster has passed.

### Why we need BCP

**Disaster might occur anytime**, so we must be prepared. Depending on the size and nature of the business, we design a plan to minimize the disruption of disaster and keep our business competitive.

**Business nowadays depends heavily on IT.** With the emergence of e-business, many businesses can't even survive without operating 24 hours per day and 7 days a week. A single downtime might mean disaster to their business.

Therefore, the traditional **DRP**, which focuses on restoring the centralized data centre, **might not be sufficient**. A more comprehensive and rigorous BCP is needed to achieve a state of business continuity where critical systems and networks are continuously available.

### BCP Program Coordinator

- Maintains plan
- Manages process modifications
- Has management support

> Normally BC Coordinator will be responsible for maintaining the BCP.
> However, their job is **not updating** the plan.
> Their job is to carry out review periodically by distributing relevant parts of the plan to the owner of the documents and ensure the documents are updated.

### BIA (Business Impact Analysis)

A systematic process that determines and evaluates the potential effects of an interruption to critical business operations as a result of a disaster, an accident, or an emergency

Ascertains the recovery time and recovery requirements for various disaster scenarios

The underlying assumption in a BIA is that while each component of an organization depends on the continuous functioning of every other component, some components are more crucial than the others. Hence, these critical components should receive a larger funding and their recovery should be prioritized in the wake of a disaster

### BCP Phases

#### Project Initiation

- Define BC Objective and Scope of coverage.
- Establish a BR Steering Committee.
- Draw up BR Policies.

#### Business Analysis (Business Impact Analysis)

- Perform Risk Analysis and BIA (Business Impact Analysis).
- Consider Alternative BC Strategies.
- Carry out Cost-Benefit Analysis and select a Strategy.
- Develop a BC Budget.

#### Design and Development (Designing the Plan)

- Set up a Business Recovery Team and assign responsibility to the members.
- Identify Plan Structure and major components
- Develop Backup and Recovery Strategies.
- Develop Scenario to Execute Plan.
- Develop Escalation, Notification and Plan Activation Criteria.
- Develop General Plan Administration Policy.

#### Implementation (Creating the Plan)

- Prepare Emergency Response Procedures.
- Prepare Command Center Activation Procedures
- Prepare Detailed Recovery Procedures.
- Prepare Vendors Contracts and Purchase of Recovery Resources.
- Ensure everything necessary is in place
- Ensure Recovery Team members know their Duties and Responsibilities

#### Testing

- Exercise Plan based on selected Scenario.
- Produce Test Report and Evaluate the Result.
- Provide Training and Awareness to all Personnel.

#### Maintenance (Updating the Plan)

- Review the Plan periodically.
- Update the Plan with any Changes or Improvement.
- Distribute the Plan to Recovery Team members (include a physical copy).

### BCP Benefits

#### Business Survival

- Prepare for the worst. If well practiced, staff and management will be able to respond to an incident appropriately
- Resources necessary to support the business through an incident will be identified and available
- Any alternative premises and resources will be ready for use

#### Risk management

- Identify, manage and mitigate as many risks as possible
- Reduce the risks where necessary
- Promotes a safer working environment and improves working conditions

#### Responsibility

- A company that takes BCP seriously will be a more attractive proposition for bankers, investors, insurers, customers and employees
- A business with a BCP will have responsible management

#### Employee satisfaction

- A sound working environment
- Welfare and safety concerns of the employee addressed
- A BCP shows your employees that they are important to the survival of the company
- Training exercises and drills are vital to the successful implementation of a BCP

### Business Continuity Planning and the Role of IT (video)

Prasad Ramakrishnan, CIO of Freshworks, describes how his team was able to take a 2500+ workforce fully remote in a week, in session with the host Alan Berkson.

He provides expert insights into how IT can help adapt and transition your business seamlessly into the new normal, in light of the coronavirus pandemic.

[Business Continuity Planning and the Role of IT [Interview] | Digital workplace best practise](https://www.youtube.com/watch?v=Ke5WmV0pn0c)

## U7P10: RPO (Recovery Point Objective)/RTO (Recovery Time Objective)

**RPO** is essentially how far back your backups should stretch.

**RTO** is the tolerance for down-time after an incident event, before recovering.

**MTD** (Maximum Tolerable Downtime) is the longest acceptable time after an incident event, and any time after that is non-acceptable.

You want the RPO and RTO to be as close to the event as possible.

### Other definitions

- **MTTF**: Mean Time To Failure (time between last failure repaired, to new failure)
- **MTTD**: Mean Time To Diagnose (time between starting diagnosis of failure, until repairing)
- **MTTR**: Mean Time To Repair (time between starting repairing of failure, until fixed)
- **MTBF**: Mean Time Between Failures (time between ending of last failure and start of current failure) = MTTF + MTTD + MTTR

### BCP Goals

- Analyzing the potential risks and losses
- Enabling the risk management process to lessen the prospect of a complete shutdown in the event of a disruption
- Prioritizing safety, health, and welfare of the organization and its staff
- Minimizing infrastructural damage in the event of a disaster
- Restoring business conditions to the pre-disaster levels
- Maintaining vital documents and details such as telephone numbers, employee details, vendor details, and client details
- Providing staff training, building awareness, and promoting disaster preparedness

### DRP Goals

- Reduce the overall organizational risk
- Alleviate the concerns of the senior management
- Ensure compliance with regulations
- Provide a rapid response after a disruption

### Guidelines for DR Implementation

- Ensure that team managing an event can act:
  - Quickly.
  - Consistently.
  - Without interference.
- Ensure that the team can escalate issues to higher levels of management.
- Categorize potential events as non-incidents, incidents, or severe incidents.
- Implement a DRP that can quickly restore critical systems to normal.
- Choose a short term or long-term approach to your recovery response.
- Establish a single, clear line of communications with stakeholders.
- Ensure personnel refer outside parties with questions to communications team (leaving them with no information makes media just publish anything).
- Use a "call tree" to accurately and efficiently spread information to personnel.
- Document all communication procedures.
- Consult legal counsel/insurance agents during restoration process.

## U7P12: Resources

Books:

- Crisis Management, by Regina Phelps
- The Manager's Guid to Enterprise Security Risk Management: Essentials of Risk-Based Security, by Brian J. Allen
- Effective Crisis Management, by Sarah Armstrong-Smith

Links:

- [NCSC: Principle D1 Response and recovery planning](https://www.ncsc.gov.uk/collection/cyber-assessment-framework/caf-objective-d/principle-d1-response-and-recovery-planning)
