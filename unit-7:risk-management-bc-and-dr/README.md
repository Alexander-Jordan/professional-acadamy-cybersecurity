# Unit 7: Risk Management, BC & DR

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
