# SOC Level 1 — Security Orchestration, Automation and Response (SOAR)

**Platform:** TryHackMe  
**Learning path:** SOC Level 1  
**Room:** SOAR  
**Status:** Completed  
**Focus:** Security workflows, alert enrichment, playbooks and human oversight

## Overview

Following practical rooms on endpoint detection and response (EDR), Splunk and Elastic Stack, I completed a room exploring **Security Orchestration, Automation and Response (SOAR)**.

The room helped me understand how a Security Operations Centre (SOC) can connect tools, automate repetitive work and coordinate incident response. I was particularly interested in where automation is useful and where an analyst still needs to make a judgement call.

This is a **learning reflection**, not a walkthrough. It intentionally excludes TryHackMe flags, challenge answers and the room's specific workflow configuration.

## Key concepts

### SIEM versus SOAR

My earlier Splunk and Elastic Stack exercises focused on getting useful information from large collections of logs. Those exercises helped me understand how centralised data, queries and visualisations support investigations.

**SIEM** (Security Information and Event Management) focuses on collecting and analysing security events, correlating activity and generating detections or alerts. **SOAR** builds on information from security tools by coordinating workflows and automating suitable actions.

One lesson for me was that collecting logs is not the same as having an effective detection and response capability. Tools need appropriate configuration, integrations, detection logic and operational processes to be genuinely useful.

### The three parts of SOAR

- **Orchestration:** Connecting systems such as SIEM, threat intelligence, endpoint security, identity management and ticketing platforms.
- **Automation:** Reducing repetitive manual work, such as gathering alert context, looking up indicators and updating records.
- **Response:** Helping teams carry out documented actions consistently, with approvals and safeguards where necessary.

### Playbooks and consistent investigations

A **playbook** defines a repeatable response workflow for a type of security event. Depending on the environment, a playbook might gather evidence, enrich an alert, update a case, request analyst review or initiate an authorised containment step.

The important principle is not to automate everything. Actions such as disabling an account or blocking a connection can have business consequences, so decisions should follow organisational policy, appropriate testing and approval requirements.

## Practical learning

The exercise involved a simulated security workflow where I had to think through which types of work were suitable for automation and which required analyst involvement.

It made me consider several distinct areas:

- **Case management:** Keeping incident information accurate, timely and available to the right people.
- **Threat intelligence:** Bringing contextual information into an investigation without requiring analysts to repeat every lookup manually.
- **Data extraction:** Collecting relevant indicators and evidence, while recognising that unfamiliar results may need human interpretation.
- **Reputation checks:** Using automated lookups to support, rather than replace, evidence-based decisions.
- **Response actions:** Understanding why potentially disruptive changes need suitable safeguards and, in some cases, human approval.

I did **not** get everything right on my first attempt. I revisited my choices, thought about the consequences of each action and adjusted my approach. Working through those mistakes was one of the most useful parts of the room, especially as automation was a relatively unfamiliar area for me.

## Personal reflection — connecting SOAR to the service desk

Several points reminded me of my work as an **IT Service Desk Analyst**.

### Documentation and handovers

I've seen firsthand how incomplete ticket notes or undocumented procedures can slow down an investigation, especially when another analyst takes ownership. Recording **what was done, why it was done and what needs to happen next** makes handovers easier and reduces duplicated work.

SOAR reinforced the value of consistent case updates and repeatable processes. Automation can help with routine record-keeping, but the information still needs to be accurate and meaningful.

### Runbooks and developing confidence

When I first started on the service desk, I regularly relied on documented procedures. As my experience grew, I became more comfortable interpreting situations and deciding which steps were relevant. I can see a similar progression in SOC work: playbooks provide structure, while experience helps analysts understand when further investigation or escalation is needed.

### Alert fatigue and disconnected tools

I could relate to the challenge of high workloads and the importance of having tools that work together. SOAR showed me how automating repetitive enrichment and case-management tasks may give analysts more time to focus on interpreting evidence and assessing risk.

I also realised that owning a security tool is only part of the solution: integrating, configuring, testing and maintaining it are essential to making it useful operationally.

## Skills and knowledge developed

- Understanding the distinction between SIEM and SOAR.
- Recognising how security tools can be orchestrated into workflows.
- Identifying opportunities for safe, repeatable automation.
- Appreciating the role of playbooks, documentation and case management.
- Understanding why analyst validation and human oversight remain important.
- Using trial and error to review and improve decisions in a simulated environment.

## Key takeaway

The most important thing I learned is that **SOAR is not about replacing analysts; it is about helping analysts work more consistently and efficiently**. Automation can reduce repetitive effort, while people remain responsible for context, judgement, escalation and appropriate control of high-impact actions.

After completing practical rooms involving **EDR, Splunk, Elastic Stack and SOAR**, I'm finding that I particularly enjoy the analytical and investigative side of defensive cybersecurity. This room helped connect the tools I have been learning about into a broader picture of how a SOC operates.

---

*This is a personal account of learning in a simulated TryHackMe environment. It is not a claim of production SOC experience. Lab-specific answers, flags and solution sequences have been omitted.*
