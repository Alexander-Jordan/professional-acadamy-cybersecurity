# Unit 10: Open-Source Intelligence (OSINT) & Social Engineering

## Summary

- Social Engineering
- Open-Source Intelligence
- Demo
- Tools & Resources

## U10P1: Unit Introduction

Learning outcomes:

- Social Engineering
- Open-Source Intelligence
- Demo
- Tools & Resources

## U10P2-P3: Social Engineering and video

> All techniques aimed at talking a target into revealing specific information or performing a specific action for illegitimate reasons.
The practice of using deception and trickery against human beings as a method of attack.

### Techniques

- Pretexting
- Baiting
- Shoulder surfing
- Tailgating/Piggybacking
- Dumpster diving
- Phishing

A social engineer could use ...

- Phishing: to get passwords, or use malware/exploit drop
- Vishing (voice): to gain more information or even passwords
- Physical: to gain access to premise, network, sensitive information

### Pretexting

A false justification for a specific course of action, to gain trust and trick the victim.

Example: the attacker claims to work for IT support and requests the target's password for maintenance purposes.

Proper identification and authentication processes, policies and trainings should be in place to circumvent such attacks.

### Baiting

Involves luring the victim into performing a specific task by providing easy access to something the victim wants.

Example: a USB flash drive infected with a keylogger and labelled "My private pics" left on the victim's doorstep.

Security policies such as an air gap and the blocking of non-authorized software and hardware will thwart most attempts, though staff should also be reminded not to trust unknown sources.

### Rules of influence

#### Reciprocity

People tend to return the favour if they see the value in what has been offered.
This is used a lot by intelligence agents and police to coerce their target into cooperation.

#### Commitment

If people commit, orally or in writing, to an idea or goal, they are more likely to honour that commitment because they have stated that the idea or goal fits their self-image.

#### Social proof

People will do things that they see other people doing.
There have been studies conducted which have successfully convinced people in a group that a red object is blue.

#### Authority

People will tend to obey authority figures, even if they are asked to perform objectionable acts.
In the workplace this is driven also by the company culture.

#### Likeability

People are easily persuaded by other people whom they like.
If you combine this with trust, the effect is compounded.
Always be wary of the attacker who comes at you with a smile.

#### Urgency

People are influence by fear of loss, or negative impacts to missing deadlines.
This creates urgency, where human error is likely to be exploited the most, e.g. ransomware.

### Video

[Hannibal Lecter - Social Engineering (Pretexting)](https://www.youtube.com/watch?v=4rDTnRGmVBs)

## U10P4-P5: Vishing and video

[Hacking challenge at DEFCON: Vishing part](https://www.youtube.com/watch?v=fHhNWAKw0bY&t=66s)

## U10P6-P7: Shoulder Surfing

### Shoulder Surfing

Wikipedia:

> Observation may be conducted remotely or at close range by covertly looking over the target's shoulder.
> For example, a shoulder surfer may spy on a person entering their PIN in an ATM.

### Dumpster Diving

Attackers searching trash/discarded materials for sensitive data to exploit.

### Tailgating/Piggybacking

The act of following an authorized person into a restricted area or system.

Example: the attacker, dressed as an employee, carries a large box and convinces the victim, who is an authorized employee entering at the same time, to open the door of the data-centre using the victim's RFID pass.

Access to non public areas should be controlled by access policies and/or the use of access control technologies, the more sensitive the area the stricter the combination.

The obligation to wear a badge, the presence of a guard and actual anti-tailgating doors such as mantraps with RFID access control should be sufficient to deter most attackers.

### Phishing

Persuade potential victims into divulging sensitive information such as credentials, or bank and credit card details.

They involve a combination of social engineering and deception.

The attack usually takes the form of SPAM mail, malicious Web sites, email messages, or instant messages, appearing to be from a legitimate source such as a bank, or a social network.

Often use scare tactics or urgent requests.
These fraudulent messages are usually not personalized and may share similar generic properties.

#### Different phishing techniques

- Pharming: fake website
- Spear phishing: specifically targeted
- Whaling: targeting important people
- Smishing: SMS phishing
- Lishing: LinkedIn phishing

#### How to spot a phishing attempt

- Unusual requirements
- Requiring respect for authority
- Threat of negative consequences
- Urgency
- Giving praise and flattery
- Offering something for nothing
- Seems too good to be true, etc...

### Social engineering red flags

#### Email

Look if any of the following looks suspicious:

- From
- To (CC)
- Hyperlinks
- Content
- Attachments
- Subject
- Date/time

#### URLs

These are red flags for a rouge URL:

- Look-alike domains
- URL domain name encoding
- Shortened URLs
- Domain mismatches
- Strange originating domains
- Overly long URLs
- File attachment is an image/link
- Open redirects (at the end of URL)

## U10P8: Phishing Quiz

[Google: Phishing Quiz](https://phishingquiz.withgoogle.com/)

## U10P9: Recommendations

- Frequent awareness campaigns: posters, presentations, emails, information notes.
- Staff training and exercises.
- Penetration tests to determine an organization's susceptibility to social engineering attacks, reporting and acting upon the results.
- Never answer a message that appears to be phishing. Rather, try to make contact with either your bank, web site, or IT department yourself.
- In all cases, never follow links from an unsolicited message, but rather use bookmarks or type the web site's address yourself. When in doubt, ask a professional.
- Review KnowB4 Phishing eBook in your notes.

## U10P10-11: OSINT (Open Source Intelligence)

Michael Bazzell, 2016:

> Any intelligence produced from publicly available information that is collected, exploited, and disseminated in a timely manner to an appropriate audience for the purpose of addressing a specific intelligence requirement.

### Who uses this type of information?

- Military
- Law Enforcement
- Criminals
- Business
- Government
- Spies
- Private Investigators

### Output Examples (For what is this research used?)

- Individual Privacy Report
- General Investigation: Insurance, Cyber Attacks
- Social Media Landscape Report
- Travel Risk/Country Analysis
- Pen Testing
- Damage Limitation/Brand Protection (PR)
- Due Diligence

### Sources

- Public Records: Government databases, financial filings.
- Media: News articles, press releases.
- Internet: Websites, blogs, social media.
- Geospatial Information: Maps, satellite imagery.
- Professional and Academic Publications: Research papers, whitepapers.

### Tools

- Maltego: Visual link analysis tool.
- Shodan: Search engine for Internet-connected devices.
- Google Dorks: Advanced search techniques using Google.
- Social Media Tools: Tools like TweetDeck, Social-
- Searcher for social media monitoring.
- Others: Spiderfoot, Recon-ng, FOCA.

### From you real name

Using tools such as social media, search engines, people search, or data breaches, they can gain information about you such as:

- Address
- Phone number
- Usernames
- Interests
- Social networks

### Resources with OSINT tools

- [Intel Techniques](https://inteltechniques.com)
- [OSINT Framework](https://osintframework.com/)

## U10P12-P13: Tools

- [Followerwonk](https://followerwonk.com)
- [Twiangulate](https://www.twiangulate.com/search/)

### Resources

- [I-Intelligence: OSINT tools and resources handbook 2020](https://i-intelligence.eu/uploads/public-documents/OSINT_Handbook_2020.pdf)
- Google tools
- Trends, reverse image.
- [Have I been Pwned](https://haveibeenpwned.com/)
- [Namechk](https://namechk.com/)
- Google Trends
- Google Alerts
- Bellingcat's Online Investigation Toolkit
- Google Dorks

#### More tools

- [CIA: World Fact Book](https://www.cia.gov/the-world-factbook/)
- Buscador OS (Not supported): New one with OSINT book.
- Waybackmachine: Internet Archive
- [Paliscope](https://www.paliscope.com/2020/11/04/200-of-our-best-osint-investigation-tools-free-download/)

#### Books

- Ghost in the wires, by Kevin Mitnick
- The psychology of online behavior, by Nicola Fox Hamilton
- People hacker: confessions of a burglar for hire, by Jenny Radcliffe

## U10P14: Further Reading

- [Talk Talk Attack](https://www.channel4.com/news/by/geoff-white/blogs/)scammers-conned-talktalk-customers-thousands-pounds
- [Spam Factory](https://geoffwhite.tech/2017/08/11/inside-the-scam-factory/)
- Identity Theft: ENISA Report
- [Stuart Peck: Diving Head First into OSINT](https://www.youtube.com/watch?v=44KeIpg55es)
- [The Role of the Human Factor: Social Engineering](https://insights.pecb.com/role-human-factor-social-engineering/)
