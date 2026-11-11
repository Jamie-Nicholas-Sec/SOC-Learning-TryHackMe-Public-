# Endpoint Detection and Response (EDR) | TryHackMe

**Platform:** TryHackMe  
**Pathway:** SOC Level 1  
**Room:** Endpoint Detection and Response (EDR)  
**Status:** Completed  
**Focus:** Endpoint visibility, threat detection, investigation, and containment

## Overview

I completed this room alongside a university lesson on disaster recovery. It introduced how **Endpoint Detection and Response (EDR)** solutions help security teams identify suspicious activity on devices, understand the sequence of events, and take action before an incident spreads.

The room combined an overview of EDR architecture with guided investigations into endpoint processes, suspicious files, and network activity.

## Key learning points

### 1. How EDR works

EDR agents (sometimes called sensors) collect security-relevant telemetry from endpoints and send it to a central management platform. This gives analysts visibility into activity that might otherwise be difficult to piece together.

Examples of telemetry include:

- **Process activity:** Executed programs and parent-child relationships.
- **Command-line activity:** Commands and scripts launched on a device.
- **Network connections:** Potentially suspicious external communication.
- **File activity:** Changes, creations, and other relevant events.
- **Registry activity:** Changes to Windows configuration and persistence-related settings.

EDR supports investigation by connecting events and providing their surrounding context.

### 2. Antivirus and EDR

I explored how EDR extends endpoint security beyond traditional malware prevention. While modern antivirus products can also use behaviour-based detection, EDR focuses heavily on continuous telemetry, investigation context, and response capabilities.

This is useful when the concern is not just a known malicious file, but a suspicious **sequence of actions** across otherwise legitimate programs.

### 3. Recognising suspicious behaviour

The room introduced several approaches to detection, including:

- Behavioural and anomaly detection.
- Indicators of compromise (IOCs) and threat intelligence matching.
- Process relationship and execution-chain analysis.
- Mapping suspicious techniques to the MITRE ATT&CK framework.

I learned why an individual event should be assessed in context. A legitimate tool or process can be used for ordinary administration or appear within a malicious sequence; the surrounding evidence helps distinguish the two.

### 4. Investigating endpoint alerts

In the guided practical exercises, I used an EDR investigation interface to review process information, supporting indicators, file activity, and network-related evidence.

The most valuable concept was following the **process tree**: understanding which process launched another can help explain how suspicious activity began and developed.

### 5. Responding to threats

EDR platforms may provide response capabilities such as:

- Isolating an affected endpoint from the network.
- Terminating a suspicious or malicious process.
- Quarantining a file.
- Collecting additional evidence or performing approved remote actions.

These actions should follow the organisation's incident response procedures, with care taken to preserve necessary evidence and avoid unnecessary disruption.

## Connection to disaster recovery

This room was relevant to our university discussion of disaster recovery because **early detection and containment can reduce the scale of an incident and support a safer recovery process**.

For example, identifying compromised endpoints and limiting their ability to communicate may help prevent further disruption while teams assess the impact and plan restoration.

However, EDR is **not a replacement for a disaster recovery plan**. Recovering services still depends on measures such as reliable backups, restoration procedures, business priorities, and recovery objectives.

## Personal reflection

I enjoyed seeing how an EDR platform combines multiple sources of evidence into one investigation. The process-tree view was particularly useful because it helped me understand the relationship between seemingly separate events.

My current IT Service Desk experience has already shown me the importance of endpoint management, troubleshooting, documentation, and escalation. This room introduced how similar investigative habits apply when the objective is identifying and containing security threats.

It also reinforced the importance of questioning the context behind an alert rather than immediately assuming every unfamiliar program is malicious.

## Skills developed

- Understanding EDR architecture and endpoint telemetry.
- Reviewing suspicious process execution chains.
- Interpreting indicators of compromise and supporting context.
- Understanding endpoint isolation, process termination, and quarantine.
- Connecting endpoint investigation to incident response and recovery.
- Recognising the role of EDR alongside other security controls.

## Conclusion

This room strengthened my understanding of how security analysts investigate endpoint threats and how timely containment can help organisations limit damage before recovery activities begin.

I intend to continue building my practical SOC investigation skills through the remaining Level 1 pathway.

---

*This is a personal learning reflection. Specific TryHackMe answers, flags, file paths, and lab indicators have intentionally been omitted.*
