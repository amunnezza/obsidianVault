# Module 1: Understand Incident Response

Domain D2.3.1, D2.3.2, D2.3.3

#### Module Objective

-   L2.1.1 Identify the terms and components of incident response.

TraNSCRIPT
Manny: Wow, it seems like we tackled a lot of topics in Chapter 1. So many ways information can be protected through policies, procedures, and physical and logical controls. 
Tasha: That's right. But as we know from reading the headlines, sometimes things go wrong. Let's find out more about the types of incidents that can happen and how cybersecurity professionals respond to them. 

# Incident Terminology

While security professionals strive to protect systems from malicious attacks or human carelessness, inevitably, despite these efforts, things go wrong. For this reason, security professionals also play the role of first responders. An understanding of incident response starts with knowing the terms used to describe various cyberattacks.
_Click on each tab to learn more._

Tab 1: Breach
The loss of control, compromise, unauthorized disclosure, unauthorized acquisition, or any similar occurrence where: a person other than an authorized user accesses or potentially accesses personally identifiable information; or an authorized user accesses personally identifiable information for other than an authorized purpose. Source: NIST SP 800-53 Rev. 5

Tab 2: Event
Any observable occurrence in a network or system. (Source: NIST SP 800-61 Rev 2)

Tab 3: Exploit
A particular attack. It is named this way because these attacks exploit system vulnerabilities.

Tab 4: Incident
An event that actually or potentially jeopardizes the confidentiality, integrity or availability of an information system or the information the system processes, stores or transmits.

Tab 5: Intrusion
A security event, or combination of events, that constitutes a deliberate security incident in which an intruder gains, or attempts to gain, access to a system or system resource without authorization. Source: (IETF RFC 4949 Ver 2)

Tab 6: Threat
Any circumstance or event with the potential to adversely impact organizational operations (including mission, functions, image or reputation), organizational assets, individuals, other organizations or the nation through an information system via unauthorized access, destruction, disclosure, modification of information and/or denial of service. Source: NIST SP 800-30 Rev 1

Tab 7: Vulnerability
Weakness in an information system, system security procedures, internal controls or implementation that could be exploited by a threat source. NIST SP 800-30 Rev 1
Tab 8: Zero Day

A previously unknown system vulnerability with the potential of exploitation without risk of detection or prevention because it does not, in general, fit recognized patterns, signatures or methods.

What does incident response in cybersecurity look like? No 911 calls have reported an incident. No ambulances or fire engines are coming to the rescue. It's up to the cybersecurity professionals to detect and respond to incidents.
*****
# The Goal of Incident Response

Every organization must be prepared for incidents. Despite the best efforts of an organization’s management and security teams to avoid or prevent problems, it is inevitable that **adverse events** (_**def: Events with a negative consequence, such as system crashes, network packet floods, unauthorized use of system privileges, defacement of a web page or execution of malicious code that destroys data.)**_ will happen that have the potential to affect the business mission or objectives.

The priority of any incident response is to protect life, health and safety. When any decision related to priorities is to be made, always choose safety first.

The primary goal of incident management is to be prepared. Preparation requires having a policy and a response plan that will lead the organization through the crisis. Some organizations use the term “crisis management” to describe this process, so you might hear this term as well.

An event is any measurable occurrence, and most events are harmless. However, if the event has the potential to disrupt the business’s mission, then it is called an incident. Every organization must have an  **incident response plan** _**(The documentation of a predetermined set of instructions or procedures to detect, respond to and limit consequences of a malicious cyberattack against an organization’s information systems(s). NIST SP 800-34 Rev 1)**_ that will help preserve business viability and survival.

The incident response process is aimed at reducing the impact of an incident so the organization can resume the interrupted operations as soon as possible. Note that incident response planning is a subset of the greater discipline of business continuity management (BCM), which we will cover shortly.

# Incident Response Priorities

Being prepared to respond to incidents can make a difference in how quickly an organization can resume operations. 

Listen to the following podcast for advice from a subject matter expert on prioritizing incident response.
file IncidenteResponsePriority.mp3
### file IncidentResponsePriority.mp3
[Download Transcript]()

Chad Kliewer: All right. Good morning, good afternoon, or good evening, depending on where in the world you're listening from. So welcome to the discussion on the importance of prioritizing responses to incidents. I'm your host, Chad Kliewer, holder of CISSP, CCSP, and current (ISC)2 member. And I'll be facilitating your experience today, and I'm extremely excited to welcome our special guest for today's discussion, Daniel Hernandez. I invited Daniel here today because he has perspectives very close to you, our listeners. Daniel's currently working towards his CISSP and has a history of about five years as a CIS admin and about a year as an information security analyst. So, I'm going to dive right in here and say, lay a little bit of groundwork on this first one here, and say that I think we talked, in our courses, that security exists to support the business operations, something that's a very important point to make for us here at (ISC)2 . You know, security is important, there are a lot of technical components to the security, but ultimately security is there to support the business and make sure the business can continue to operate safely and securely. So, what we're going to dive into specifically is a business continuity plan or BCP. And what that is really trying to do is to create an easy-to-use actionable solution to help prepare for the impact of an actual incident or even the broad range of threats occurring to an organization. Now, the business continuity plan and what it takes to keep a business operating applies—you know, we think of that often and we think of disasters often in the term of natural disasters (tornadoes, floods, hurricanes you name it), but this also, of course, includes global pandemics, it includes accidents. It could include acts of terrorism. So, when we're thinking about a business continuity plan, we're really trying to make sure that we can plan and keep the business operating from a technical perspective, but providing that technical support to the business to keep them operating with the systems, either working or not working, as effective as possible. So, we're looking at how these hazards can cause the failure and how we can keep these operating in terms of system equipment software. So, Daniel, I know you're very aware of how the BCP keeps incident response and disaster recovery in place. So, what we're here to really talk about is how, when that business continuity plan and the incident response plans fail, is how we start with disaster recovery. So, I'm just wondering, and we're speaking of disasters and I'm going to turn a little bit of a different one and I don't know how familiar you are with the, and we're going to call it a disaster, but the 2017 Equifax breach and how that impacted more than 150 million consumers. And really, Canada, US, and Britain, but from all over the world. So how do you feel, you know, and what kind of a plan do you have in place, or have you thought about, either personally or professionally, and how can you protect and how can you make sure you can continue business in the face of a breach such as Equifax? Daniel Hernandez: Well, you know, I think one of the most important pieces there in your incident response plan would be the communications portion, right? How do you communicate to those affected by the incident or the disaster that occurred? So, I think those are—that's probably one of my focal points is having clear and good communication with, you know, everyone that is affected by it and, you know, just all the stakeholders within your incident response planning. I think that's a very important piece of it, too, just understanding who are the stakeholders that you need to communicate with or inform of the different stages that are there. So does that kind of—? Kliewer: Absolutely, it really does. And I think you bring out a really important part, because most of us that are looking at a career in security or are already in a career in security are very much technical-minded. We're not necessarily thinking about those non-technical pieces and it's a great point to bring that in. Absolutely, communication is key. "Communicate early, communicate often," I think is what a lot of people say about that. The other trick to that is to make sure we get those communications on the right level, to make sure we're communicating with people and not communicating to people. Now, I understand—and since we got off kind of on this communication tangents and one of the reasons, I was excited to have you as a guest, is I understand you've got some, we'll say some background or history, not necessarily in security area, but you've got some background in how to adjust that communication for the different audiences. Would you want to share that with us? Hernandez: Yeah, for sure. So, you know, growing up, often I was tasked with translating from Spanish to, or from English to Spanish and Spanish to English, you know, my parents not being native language speakers, and they relied on me for a whole lot of that. So, you know, I felt that, for the longest time, I've always been that middleman between two different parties, you know, just for a long time. And so, I think I've developed those skills throughout the years. And translating them, I mean, even from just a technical perspective, being able to, you know, communicate different issues to non-technical individuals, and now, you know, as I moved onto the security realm, now communicating the security issues to technical individuals that don't understand, you know, risk may be one of those things that they don't quite understand, and translating it into their own languages is kind of important. And I think it's something that is good to have in the field is being able to communicate to different levels, you know, doing that translation for them. Kliewer: Okay, absolutely. And I think that is absolutely key to this whole process is, like I said, that communication at the right level. And to make sure that that communication is absolutely included in the business continuity plan, incident response plans, and disaster recovery plans, which all tie in together. So, great insight there. So, I want to talk a little bit more, maybe, on the security side of things for a minute now. And I'm wondering, and as close as you can get without naming any organizations, other than we all know what the big breach is out there and that, but without naming any of your organizations or giving away any real secrets there, what kind of incident or disruption have you seen within your career and how do you think that response was? Hernandez: Well, are we allowed to talk about the “S” one? Kliewer: Absolutely, I think everybody knows all about SolarWinds. Hernandez: Yeah, so SolarWinds, you know, that was quite, I think it was something that, it was a revelation to the industry as a whole, and, well, maybe even the nation, you know, because it revealed that we're susceptible to being attacked from, you know, our trusted parties. So, you know, I think, for a lot of us, it told us that we need to do a better job at vetting our suppliers of software and hardware as part of our business continuity planning and third-party risk management. It is a big portion, you know. You have to take into account that, whenever you're doing your incident response, you have to look at, okay, you know, what is the criticality of this piece of software that has been compromised? If you need to isolate a machine that is hosting, you know, SolarWinds, how does that impact the business as a whole? You know, from us in critical infrastructure, we have to monitor our equipment continuously, so it is a great impact to not be able to have those eyes to, you know, understand what equipment is up and running, so. Kliewer: Absolutely, and I want to pick on something you said there, Daniel, just talking about being in critical infrastructure and talking about the impact. And what I want to be real clear about there is the impact and what you've got to do with that business continuity plan, that disaster recovery plan, is how does that really affect your business and how do these different pieces affect your business? It will be absolutely different for every business, I guarantee. I've also had a lot of conversations about SolarWinds with different groups. A lot of people, when that stuff happened, they said, "Okay, we just ripped it all out and we went with a different vendor." That's not always an option. If you're an internet provider, you operate a very large network, it's absolutely crucial to your operations. It's not just a monitor to see what's working and what's not, or to help you deploy patches. It's a lot more than that. It's very integral to your daily operations. So, I think our lesson there is to really look at how it integrates to your daily operations and understand that. And that's the biggest part of that business continuity plan. Remember, the business word comes first. So how does this keep the business running and how does the business keep running when you don't have it, or if you don't have it. So, do you think that that incident changed? I can tell it definitely changed the way you think about keeping, I don't want to get up on a supply chain tangent here, but I can tell it changes the way you think about the business continuity and the way we use and the way we evaluate things. Do you think that had any impact on the organization as a whole into how people think about how we use things? Hernandez: Yes, absolutely. You know, I think because, you know, working in a small, rural, you know, telecom, perspective of things may be different throughout the organization, but once they all understand what's at stake and what are some of the risks that imply or are implied with, you know, having a breach or, you know, things like that. I think it has, you know, gone all the way up to our general manager and our board, you know, to help them understand that yes, there is a priority that needs to be addressed with security, you know, and how we handle just security for the whole organization, that there's a place on the table for, you know, all of the business leaders who deal with the day-to-day operations and management of the organization, that there is a need for them to understand risk, you know, and the different risks that cybersecurity has brought in into their eyes. Kliewer: Okay, awesome. And I want to turn the conversation just a little bit, and once again, I'll lay a little bit of groundwork here. And I'm going to talk just a second about the National Institute for Standards and Technology and how they define incident response. They define preparation, detection and analysis, containment and recovery, and post-incident activities. We've talked mostly about preparation, the business continuity plan, which we know is of the ultimate importance. We're going to kind of skip the middle two because we talked, you know, I talked with some of those in a different podcast about incident response and actual incidents. But what I want to do now is fast forward to those post-incident activities. And I'm going to say this because we're mostly technical people, we like to get in, we like to fix things, we like to get out. “It's fixed now, what else is there for me to do?” So, what I'm curious about, Daniel, is I want to hear your perspective a little bit more on why the post-incident activities and what happens after you've contained an incident, after you've resumed operations—you know, when we've got to do that after-incident report or whatever. Help me understand the importance of that. Hernandez: So, you know, often, I compare security with raising a child or the upbringing of a child. So, you know, I'm a new dad, you know, nine months or so. And when an incident happens where, you know, my daughter falls and at the end, I let her go through the whole process of, you know, you have to cry and, you know, it's okay, you pamper her and do this and that, but at the end, there needs to be some growth. And so, the post-work of an incident is probably, you know, as important as the prep work that is done at the beginning, you know, that we already talked about. I believe the learning really happens there for a lot of people, is after they realize what went wrong, then the learning really happens because you have their attention fully. And at that point, you know, you can really provide them with the tools that they need to make sure that this type of incident does not happen again, because you have a timeline, and you have history to look back on and make sure that they don't forget that. Kliewer: Absolutely, because what are we doing? And it's not easy for us to do, but so what are we doing? We're looking at—when you're talking about post-incident, we're like, "Where did we mess up? What happened? Why did this happen? It shouldn't have happened." But most importantly, we're looking to feed that back to our business continuity plan to say, "Where did we miss that? What can we do to shore up our planning ahead and our business continuity first?" I think that's a great way to do it. And of course, I'm going to throw back in there again, just like what you were talking about, translating not necessarily English to Spanish and back and forth, but translating back and forth between the technical teams and the business teams to make sure that the goal on both sides are being met. And I think that's an awesome point to have. So finally, I'm going to kind of wrap up with one question and I'll give you an opportunity to share anything you want to after that. So really, one final question, and I'm curious how you feel, being part of critical infrastructure in the United States, how do you feel that entities like, and I'm going to use the example of the US-CERT, and I know there are other ones and the names are not coming to me right now, but I know there are other ones worldwide, such as the UK has another agency, Japan has their agency that handles these kind of things. And I know other countries do as well. But I'm curious how you feel that the roles that those government agencies play in your incident response and in what, you know, how do you feel their role is, and how does that plug into your plan? Hernandez: That's a good question. And I think, you know, from all the work that I've done in the last year or so, I've come to really—you know, when it comes to something critical and a critical incident or an incident that relates to a piece of either data or a system that is critical to our industry or to our organization, you know, we have to have a trust relationship with government at some point, because we, as critical infrastructure phase threats from overseas that are not local and we can't just report to the police and, you know, just that it'll actually have an impact on the threat that we're looking at. So, I believe that having those relationships with the FBI and with CISA is making sure that you can trust, you understand who are your contacts, is just of the most importance, I believe. And to have that contact information within your incident response, make sure that you have the information available for when you need it, because timeliness is, something that is critical for incident response is making sure you shorten that time. It makes a big difference at the end. Kliewer: Absolutely correct. And I'm going to put a big exclamation point after that and say, especially, not necessarily US-CERT, but when you're talking about people like the FBI or CISA within the US, or whatever your agency is in other countries, be sure you know who your contacts are and don't be afraid to document that. I'm not going to say don't be afraid, do document it. Definitely do. Because I'll guarantee you, I don't care how many times you think about it, how many times you think you have incidents or whatever. Until that incident hits you and until you find out you have a breach, or you have a large incident sitting in front of you, you realize that no matter what you thought about, it just went out the window. And if you don't have that documented, you're still going to run around in circles and wonder what to do. So, when you say that and having those steps documented is absolutely key as part of the business continuity and your incident response and your disaster recovery. So, make sure you've got those documented and where you're going with those. So that's a great note to wrap up on, Daniel. Do you have any last-minute pieces of advice that you'd want to share? Hernandez: Just keep going, that's all I got to say. You know, because I think a big portion of your audience may be entry level. And I just want to say, you know, don't be afraid that, you know, you don't have to know all of it from the get-go. You know, there's always great mentors like Chad himself and information security that you can look up to and gain a lot from, you know, as you continue your journey in information security. It is a great field to be in. It's very rewarding for a lot of us. So that's all I got. Kliewer: I love that, to finish up on a positive note. After we talked about all the bad stuff, it's always great to say, yeah, absolutely, using Daniel's words, "Keep pressing forward. Keep moving forward." Things will happen, just make sure you learn from them and move on. I think that's a great piece of advice. And with that, we're going to wrap up here and I hope you've enjoyed our discussion. And again, I want to say many, many thanks to our special guest, Daniel Hernandez, for volunteering his time and to share his experiences with us here today. And thank you very much for listening.
****
# Components of the Incident Response Plan

The incident response policy should reference an incident response plan that all employees will follow, depending on their role in the process. The plan may contain several procedures and standards related to incident response. It is a living representation of an organization’s incident response policy.

The organization’s vision, strategy and mission should shape the incident response process. Procedures to implement the plan should define the technical processes, techniques, checklists and other tools that teams will use when responding to an incident.

To prepare for incidents, here are the components commonly found in an incident response plan:

_Select each plus sign hotspot to learn more about each topic._![[frame.png]]

# Preparation
-   Develop a policy approved by management.
-   Identify critical data and systems, single points of failure.
-   Train staff on incident response.
-   Implement an incident response team. (covered in subsequent topic)
-   Practice Incident Identification. (First Response)
-   Identify Roles and Responsibilities.
-   Plan the coordination of communication between stakeholders.
    -   Consider the possibility that a primary method of communication may not be available.

# Detection and Analysis
-   Monitor all possible attack vectors.
-   Analyze incident using known data and threat intelligence.
-   Prioritize incident response.
-   Standardize incident documentation.

# Containment
-   Gather evidence.
-   Choose an appropriate containment strategy.
-   Identify the attacker.
-   Isolate the attack.
# Post-Incident Activity
-   Identify evidence that may need to be retained.
-   Document lessons learned.

Retrospective

-   Preparation
-   Detection and Analysis
-   Containment, Eradication and Recovery
-   Post-incident Activity

****

# Consulting with Management

###  video ConsultingWithManagment.mkv

Narrator: The first part of preparation is identifying the critical information that needs protection and avoiding any single point of failure. This means that if we have something particularly important, but it is protected by just one door, we create multiple layers of protection to reduce the likelihood of a successful attack. We will talk more later about the principle of defense in depth, but like a fortress, the more layers of defense we have, the more difficult it will be for attackers who are trying to break through. It is important to train staff in incident response so that everyone knows what to do. Training can include simulations and scenarios so teams can practice their response and learn to coordinate communication among the different stakeholders of the organization. That includes colleagues, superiors, the owners of the information and customers as well. We need to consider what types of communication will be available, because we cannot communicate the same information to everyone. Some material will be confidential, and some will be useful only to certain people and not to the press or outside individuals. When it comes to detection and analysis, we need to monitor the attack vectors, how the attack was made and what technology was used. It is important to standardize the incident documentation, because in a group of people, each will have their own idea of how to record activities and procedures. For the consistency of the organization and our responsibility to the data owners, we need to have a standardized incident response, where each person knows exactly what needs to be done and in what sequence. This makes it easier to prioritize the response, because each person has their own tasks and knows how to take care of their own responsibilities then communicate appropriately with others concerned. Next, we need to find the appropriate containment strategy, identify the attackers and how they penetrated our defenses, and isolate the attack, making sure it does not go any further or do additional damage. After the incident, we identify evidence that may need to be retained then, often, there is an internal audit of what occurred. External investigation may also be required, especially in major cyberattacks where law enforcement is involved. Lessons learned must be documented. Perhaps, it will be found that we responded better than during a previous attack, but we still need to improve preparation or detection analysis. Often, these post-incident activities are subject to regulatory requirements, and certain documentation must be submitted. This is especially important if the compromised critical information is protected by law.
****
# Knowledge Check: Incident Response Terms

![[drak.png]]
****

# Incident Response Team

Along with the organizational need to establish a [Security Operations Center (SOC)]()
>[!Security Operations Center (SOC)]-
>A centralized organizational function fulfilled by an information security team that monitors, detects and analyzes events on the network or system to prevent and resolve issues before they result in business disruptions.

is the need to create a suitable incident response team. A properly staffed and trained incident response team can be leveraged, dedicated or a combination of the two, depending on the requirements of the organization. 

Many IT professionals are classified as first responders for incidents. They are the first ones on the scene and know how to differentiate typical IT problems from security incidents. They are similar to medical first responders who have the skills and knowledge to provide medical assistance at accident scenes and help get the patients to medical facilities when necessary. The medical first responders have specific training to help them determine the difference between minor and major injuries. Further, they know what to do when they come across a major injury. 

Similarly, IT professionals need specific training so they can determine the difference between a typical problem that needs troubleshooting and a security incident that they need to report and address at a higher level. 

A typical incident response team is a cross-functional group of individuals who represent the management, technical and functional areas of responsibility most directly impacted by a security incident. Potential team members include the following:

-   Representative(s) of senior management
-   Information security professionals
-   Legal representatives
-   Public affairs/communications representatives
-   Engineering representatives (system and network)

Team members should have training on incident response and the organization’s incident response plan. Typically, team members assist with investigating the incident, assessing the damage, collecting evidence, reporting the incident and initiating recovery procedures. They would also participate in the remediation and lessons learned stages and help with root cause analysis.

Many organizations now have a dedicated team responsible for investigating any computer security incidents that take place. These teams are commonly known as computer incident response teams (CIRTs) or computer security incident response teams (CSIRTs). When an incident occurs, the response team has four primary responsibilities:

-   Determine the amount and scope of damage caused by the incident.
-   Determine whether any confidential information was compromised during the incident.
-   Implement any necessary recovery procedures to restore security and recover from incident-related damage.
-   Supervise the implementation of any additional security measures necessary to improve security and prevent recurrence of the incident.

****

# Incident Response in Action

### VIDEO IncidentResponseInAction.mkv

Tasha: It's a slow day at the coffee shop, and Keith notices that Nate seems distracted and worried. Keith: What's wrong? You don't seem like yourself today. 
Nate: Oh. Well, I just got a lot on my mind. Did you hear what happened to our neighbors? 
Keith: What do you mean? 
Nate: Well, last Friday night when that storm was happening, some water got into the hardware store and damaged their front cash register. I mean, they were trying to open Saturday morning, and then when they couldn't, they had to close the shop and wait for it to be repaired. Could you imagine closing the store for an entire weekend? Keith: No, that's our busiest time. 
Nate: Mm-hmm. 
Keith: Huh, if only the hardware store had an extra cash register, they could have used that instead of having to close it down. 
Nate: Exactly, and then on top of that, there was a break-in at the bakery. Their laptop got stolen. I mean, think about all the banking and customer information that was on that thing. 
Keith: Yeah, that's scary. 
Nate: Yeah. 
Keith: I wonder if they would've had the laptop in the safe, it wouldn't have got stolen. I just hope the data on the laptop was encrypted or a password or a passcode was needed to decrypt it. 
Nate: Wait, wait, what are you talking about? 
Keith: Oh, it's just talk with Susan about securing data. Anyway, I wonder where that laptop is now. 
Nate: Who knows? But, you know, it got me thinking what we can do to kind of make sure things like that don't happen here. 
Keith: Huh. Susan says it's inevitable that adverse events can happen that will affect the business. You know what we need? An incident response plan. 
Nate: What is that? 
Keith: Don't worry about it. I got it. 
Nate: Okay. 
Tasha: Later that day, Keith gets Nate and Sandra together. 
Keith: Hey all, thanks for coming. Look. This is what we have here. Well, first of all, Susan taught me that we need to be prepared with an incident response plan so we can reduce the impact of an incident. So, I've written one, and the three of us get to be the incident response team. 
Sandra: Okay, Keith. Thanks. Uh, so what do you need us to do? 
Keith: Well, when an incident occurs, the three of us will determine the amount and scope out any damage, including whether or not any confidential information was leaked. Then, we'll have to implement recovery procedures and restore any damage that occurred. It's all in the plan here. 
Nate: Cool, Keith. Hey, thanks for taking this on. I really look forward to reading it. Sandra: Yeah, me too. 
Keith: Great. Great. Because we all have to be familiar with this plan. I made a checklist for every employee, and it lets them know what they're responsible for in case of an incident and how to contact each other. 
Nate: You know, we can make this the agenda for our next staff meeting. Keith: Yes. I actually want to schedule some training sessions for everyone, so we all know how to communicate if an incident occurs. 
Sandra: This is such a relief. Thank you, Keith. I feel much better about things now. 
Nate: Yeah, good job, man.
****
# Video Knowledge Check: Application of Incident Response

IncRespApplication.mkv