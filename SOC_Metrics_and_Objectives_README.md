# SOC Metrics and Objectives | TryHackMe

**Platform:** TryHackMe  
**Pathway:** SOC Level 1  
**Room:** SOC Metrics and Objectives  
**Status:** Completed  
**Focus:** SOC performance metrics, response times, and continuous improvement

## Overview

This room explored how Security Operations Centres (SOCs) measure performance and use those measurements to improve alert handling, detection capability, and response processes.

One of my main takeaways was that generating alerts is only part of security monitoring. Alerts must also reach analysts in time, be investigated accurately, and lead to an appropriate response.

## Key learning points

### 1. Alert quality and workload

I learned about several measurements used to understand alert volumes and detection quality:

- **Alert Count (AC):** The number of alerts received.
- **False Positive Rate (FPR):** The proportion of alerts determined to be false positives.
- **Alert Escalation Rate (AER):** The proportion of alerts passed on for further investigation.
- **Threat Detection Rate (TDR):** The proportion of known threats that detection controls successfully identify.

These metrics are most useful when interpreted together. For example, a high alert count does not necessarily indicate good detection, and a very quiet dashboard is not automatically reassuring: it may warrant checking whether log collection or detection rules are working correctly.

Excessive false positives can create alert fatigue, making genuine threats harder to identify among routine activity.

### 2. Detection and response times

I explored three time-based measures:

- **Mean Time to Detect (MTTD):** How long it takes to identify malicious activity.
- **Mean Time to Acknowledge (MTTA):** How long it takes an analyst to acknowledge an alert.
- **Mean Time to Respond (MTTR):** How long it takes to respond to an incident, according to the organisation's defined measurement window.

The exercises reinforced that delays can occur at different stages. Improving one stage does not automatically fix the others.

### 3. Finding causes and suggesting improvements

I reviewed simulated SOC performance problems involving delayed detection, slow response, and excessive false positives. Possible improvements included:

- Reviewing log collection and detection rule schedules.
- Improving real-time alert notification and workload distribution.
- Tuning noisy rules after confirming which activities are genuinely benign.
- Maintaining clear investigation and containment procedures.
- Coordinating improvements between SOC analysts, engineers, and management.

I also learned that metrics are indicators for investigation rather than guarantees. Targets vary between organisations, threat types, and operational requirements.

## Personal reflection: Connections to IT service desk work

This room felt particularly relevant to my current role as an IT Service Desk Analyst.

On the service desk, we monitor ticket queues, prioritise incidents, follow service level agreements (SLAs), and escalate work when necessary. A large backlog or major incident can place pressure on analysts to process work more quickly, making accurate documentation and prioritisation even more important.

The SOC has similar operational pressures, but missed or delayed responses can carry significant security consequences. I found it useful to connect the metrics discussed in this room with the importance of timely triage, clear ownership, and effective escalation in my own work.

## Skills developed

- Understanding SOC alert and performance metrics
- Interpreting false positive and escalation rates
- Understanding detection, acknowledgement, and response delays
- Recognising alert fatigue and workload pressure
- Identifying opportunities for detection and workflow improvements
- Relating SOC processes to IT service management and SLAs

## Conclusion

This room helped me appreciate that effective security operations require more than technical detection tools. Analysts, engineers, processes, and management all contribute to reducing response delays and improving detection quality.

As I continue through the SOC Level 1 pathway, I want to build on this understanding through further practical investigations and incident-handling exercises.

---

*This public writeup reflects my learning. Specific TryHackMe challenge answers, scenario solutions, and flags have been omitted.*
