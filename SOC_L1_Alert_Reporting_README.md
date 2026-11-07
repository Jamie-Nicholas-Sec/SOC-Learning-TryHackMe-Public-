# SOC L1 Alert Reporting | TryHackMe

**Platform:** TryHackMe  
**Pathway:** SOC Level 1  
**Room:** SOC L1 Alert Reporting  
**Status:** Completed  
**Focus:** Alert documentation, escalation, and communication

## Overview

This room introduced the importance of accurate alert reporting within a Security Operations Centre (SOC). An L1 analyst's responsibility is not only to investigate an alert but also to record the evidence and reasoning clearly enough for another analyst to continue the investigation when escalation is required.

I explored how reporting, escalation, and communication work together to support incident handling and maintain a reliable record of security events.

## Key learning points

### 1. Writing a useful alert report

An effective report should explain the activity, rather than simply label it suspicious. I practised using the **5 Ws** to structure findings:

- **Who:** Accounts, users, devices, or processes involved.
- **What:** The event or behaviour that triggered the alert.
- **When:** The relevant timestamp and sequence of events.
- **Where:** The affected system, application, or environment.
- **Why:** The evidence supporting the assessment and why the activity warrants attention.

Good reports should also distinguish observed facts from assumptions, explain the potential impact, and record any action already taken.

### 2. Assessing supporting evidence

The exercises involved reviewing simulated security alerts, including suspicious email activity and potentially malicious host behaviour. This reinforced the need to examine available indicators and context before deciding whether activity is benign, suspicious, or requires further investigation.

### 3. Escalation to L2

I learned how an L1 analyst can pass an alert to an L2 analyst for deeper investigation. The value of escalation depends on the quality of the handover: a clear summary, relevant evidence, reason for concern, and actions already attempted can prevent duplicated work and reduce delays.

### 4. Communication and accountability

The room also considered situations such as urgent alerts, unavailable colleagues, incomplete logs, and discovering that an earlier assessment may have been incorrect. These scenarios highlighted the importance of following escalation procedures, communicating promptly, and correcting mistakes rather than allowing a potentially significant alert to go unaddressed.

## Reflection: Connecting SOC work to my service desk experience

One aspect that stood out was how closely SOC reporting and escalation resemble the first-line and second-line processes I use in my current IT service desk role.

On the service desk, a useful ticket needs accurate notes, troubleshooting history, and a clear explanation of why further assistance is required. In a SOC, the same discipline applies, but the evidence may involve security alerts, logs, suspicious activity, and potential threats to an organisation.

This room helped me recognise that skills I already use professionally - documenting incidents, communicating with other teams, and escalating appropriately - are transferable to an entry-level SOC analyst position.

## Skills developed

- Structured security alert documentation
- The 5 Ws approach to reporting
- Evidence-based alert assessment
- L1-to-L2 escalation and handover
- Clear communication and incident recordkeeping
- Recognising the importance of reviewing and correcting assessments

## Next steps

I intend to build on these foundations as I progress through TryHackMe's SOC Level 1 pathway, particularly by developing my confidence in analysing logs, identifying suspicious patterns, and explaining findings clearly.

---

*This is a personal learning reflection. Specific lab solutions, flags, and challenge answers have been intentionally omitted.*
