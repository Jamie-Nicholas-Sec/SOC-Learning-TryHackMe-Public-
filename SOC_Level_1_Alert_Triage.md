# SOC Level 1 — Alert Triage

**Platform:** TryHackMe  
**Learning path:** SOC Level 1  
**Topic:** SOC L1 Alert Triage  
**Completed:** November 2026  
**Format:** Personal learning reflection (non-spoiler)

## Overview

This room introduced me to the practical workflow of a Level 1 Security Operations Centre (SOC) analyst: reviewing a queue of security alerts, deciding what needs attention, investigating the available context and documenting a reasoned verdict.

As someone already working in IT support, I found the similarities with incident and ticket management particularly interesting. The environment and the threats are different, but the underlying habits — ownership, prioritisation, evidence gathering and clear notes — are familiar.

## Tools and concepts explored

| Technology | Role in a SOC |
| --- | --- |
| **SIEM** (Security Information and Event Management) | Collects and correlates security events and provides visibility into potentially suspicious activity. |
| **EDR** (Endpoint Detection and Response) | Monitors endpoint behaviour and supports the investigation and response to threats affecting devices. |
| **NDR** (Network Detection and Response) | Provides insight into suspicious network activity and possible threats moving across networks. |
| **SOAR** (Security Orchestration, Automation and Response) | Helps coordinate workflows and automate approved parts of investigation and response. |
| **Case / ticket management** | Records alert ownership, investigation notes, status changes, decisions and escalation. |

These tools complement each other. A SOC may use several separate consoles or centralise aspects of its workflow, depending on its architecture and operating procedures.

## Understanding alert information

I practised interpreting the information presented in an alert, including:

- **Timestamp:** When the event occurred and when the detection was generated.
- **Name and description:** A summary of the behaviour that triggered the detection.
- **Severity:** The initial indication of potential risk, which still needs analyst assessment.
- **Status and assignee:** Whether an alert is new, being investigated, pending or resolved, and who owns it.
- **Evidence and context:** Relevant users, devices, processes, network activity and surrounding events.
- **Verdict:** Whether the investigation supports malicious activity, benign activity or a need for further review.

Understanding these fields helps an analyst avoid duplicate work, identify the right next action and leave an evidence trail for colleagues.

## How I think about triage

An important lesson was that **a high-severity label does not automatically make an alert a confirmed attack**, while a lower-severity alert should not be ignored if the available evidence suggests serious impact.

When deciding what deserves attention, I would consider the assigned severity, the age and progression of the activity, affected systems, potential business impact, and whether another analyst is already handling the case. An older alert can represent an ongoing issue, but recency alone is not a reliable measure of risk.

The room also reinforced the need to look beyond a single indicator. File names, download sources, unusual authentication patterns and volumes of network traffic can all be relevant clues; however, a familiar application or domain is not automatically safe, and unusual behaviour is not automatically malicious. The surrounding evidence should drive the conclusion.

## Connection to my IT support experience

My service desk role involves assessing incidents, recording technical details, monitoring service health and escalating issues when necessary. I also use ticket status and assignment to make sure work is clearly owned and visible to other analysts.

SOC alert triage follows a similar discipline, but applies it to suspicious security events. I particularly enjoyed the investigative aspect: forming an initial hypothesis, examining context, reaching a justified conclusion and documenting it clearly for the next person.

## Key takeaways

1. Alert triage is a combination of technical investigation, risk assessment and communication.
2. Severity labels guide prioritisation but do not replace analyst judgement.
3. True positives and false positives should be distinguished through evidence rather than assumptions.
4. Ownership, status updates and concise case notes are essential for coordinated SOC work.
5. My existing incident-management skills provide a useful foundation for a future junior SOC role.

## Next steps

I want to strengthen my ability to investigate logs and event timelines, recognise common detection patterns, and write clear incident summaries. As I continue the SOC Level 1 pathway, I will focus on understanding *why* an alert deserves escalation rather than simply memorising which button to press.

---

*This is a high-level reflection on my own learning. It intentionally omits TryHackMe room answers, flags, screenshots, specific indicators and step-by-step solutions.*
