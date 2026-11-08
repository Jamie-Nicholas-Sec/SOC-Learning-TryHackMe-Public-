# SOC Workbooks and Lookups | TryHackMe

**Platform:** TryHackMe  
**Pathway:** SOC Level 1  
**Room:** SOC Workbooks and Lookups  
**Status:** Completed  
**Focus:** Alert enrichment, contextual lookups, and repeatable triage procedures

## Overview

This room explored how Security Operations Centre (SOC) analysts use supporting information and structured workbooks to investigate alerts more efficiently and consistently.

An alert rarely provides all the information needed to reach a reliable conclusion. Understanding the users, devices, networks, and normal business activity involved can be just as important as examining the initial security event.

## Key learning points

### 1. Identity and asset inventories

I explored how analysts use identity inventories to understand the people and accounts associated with an event, and asset inventories to identify systems, device ownership, and business purpose.

Potential information sources include:

- **Identity systems:** Active Directory and Microsoft Entra ID.
- **HR and business systems:** Information about employee roles and organisational context, where access is authorised.
- **Asset management platforms:** Device ownership, system purpose, and managed endpoints.
- **SIEM and EDR platforms:** Telemetry that can help identify the activity of affected hosts.
- **Documented inventories:** Spreadsheets or other maintained records, where appropriate.

These lookups help determine whether activity is expected for a particular user or system.

### 2. Network context

I used network diagrams and addressing information to understand the role of systems and how network activity relates to their location and purpose.

An important takeaway was the distinction between **a detected malicious attempt** and **a successful compromise**. A security control can block an attack while the underlying alert still represents a true positive. The analyst's decision must be based on what was actually detected, not simply whether damage occurred.

### 3. Workbooks and repeatable investigations

SOC workbooks and runbooks provide documented investigation processes. They can help analysts gather relevant evidence, perform checks consistently, and decide when further action or escalation is needed.

The room introduced a practical pattern:

1. **Enrichment:** Gather relevant identity, asset, network, and threat intelligence context.
2. **Investigation:** Review the available telemetry and assess the activity.
3. **Decision and documentation:** Record an evidence-based assessment.
4. **Escalation:** Refer activity for deeper investigation when required, with a clear handover.

### 4. Applying workbooks to different alert types

I worked through guided examples covering:

- **Email security:** Reviewing suspicious messages and their context.
- **PowerShell activity:** Considering process behaviour, execution context, and supporting evidence.
- **Network activity:** Investigating unusual scanning behaviour and checking whether it matches authorised activity.

These exercises demonstrated why a single investigation approach does not suit every alert, even though the core principles of evidence collection, documentation, and escalation remain consistent.

## Personal reflection: Applying my service desk experience

This room stood out because several tools and procedures were familiar from my work as an IT Service Desk Analyst.

I already use Active Directory and Microsoft Entra ID in an enterprise environment, particularly when dealing with identity and access-related requests. I also regularly refer to documented procedures, previous tickets, and escalation guidance when troubleshooting unfamiliar issues.

The SOC context is different, but the underlying habits are transferable: verify the context, follow an approved process, document the evidence, and know when to escalate.

The room also helped me appreciate the value of understanding an organisation's normal systems and workflows before deciding that an event is suspicious.

## Skills developed

- Identity and asset contextual lookups
- Network diagram interpretation
- Alert enrichment using supporting data
- Differentiating malicious attempts from successful compromise
- Following investigation workbooks and runbooks
- Evidence-based decision making and escalation
- Understanding how procedures vary across alert categories

## Next steps

As I continue through the SOC Level 1 pathway, I want to strengthen my understanding of SIEM searches, event correlation, and investigative decision-making. I also intend to keep relating new concepts to the enterprise systems and escalation processes I encounter in my current role.

---

*This is a public learning reflection. Challenge answers, flags, and detailed lab solutions have been intentionally omitted.*
