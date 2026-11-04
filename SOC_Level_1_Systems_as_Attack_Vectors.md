# SOC Level 1 — Systems as Attack Vectors

**Platform:** TryHackMe  
**Learning path:** SOC Level 1  
**Topic:** Systems as Attack Vectors  
**Completed:** November 2026  
**Format:** Personal learning reflection (non-spoiler)

## Overview

This room focused on how weaknesses in software, configurations and technology supply chains can expose organisations to attack. It built on my understanding of human-focused threats by showing that **systems can be compromised without a user actively clicking a malicious link or approving a request**.

I found the distinction between a software vulnerability and a security misconfiguration especially useful, because they may need different remediation approaches.

## Types of system risk

### Software vulnerabilities

Applications, operating systems and services can contain flaws that attackers exploit. Published vulnerabilities are often tracked using **CVE identifiers**, while **CVSS** is a scoring framework that can help describe their severity. A severity score is useful context, but an organisation also needs to consider exposure, exploitability, business impact and available mitigations.

### Misconfigurations

Systems can be put at risk through insecure settings, excessive permissions, unnecessary exposed services or weak administrative controls. Unlike a defect in the underlying software, these weaknesses often require configuration changes and hardening rather than simply installing an update.

### Supply-chain compromise

Organisations rely on software from vendors, dependencies and service providers. If a trusted component or update mechanism is compromised, the consequences can spread to downstream users. This makes dependency management, supplier assurance and monitoring important parts of security.

## Defensive controls and remediation

| Control | Purpose |
| --- | --- |
| Patch and vulnerability management | Identify affected assets, assess risk, test fixes and deploy updates or compensating controls. |
| Configuration reviews | Compare settings against approved baselines and remove insecure defaults or unnecessary exposure. |
| Access restrictions and segmentation | Limit who and what can reach sensitive services, reducing potential impact. |
| Endpoint security and monitoring | Detect suspicious activity that preventive controls may miss. |
| Authorised security testing | Use vulnerability assessments and penetration tests to discover weaknesses before attackers do. |
| Staff training and change management | Help administrators configure systems securely and maintain controls over time. |

A patch is not always available, and applying one does not automatically resolve a separate configuration or access-control problem. The response should match the root cause, consider service availability and follow the relevant change and incident processes.

## Personal reflection

The scenarios encouraged me to distinguish **what is actually wrong** before deciding how to respond. For example, compromised credentials, an exposed service, an outdated component and an insecure configuration are related security concerns, but they do not all have the same solution.

That links well to my experience as an IT Service Desk Analyst. In support work, I already need to establish the symptoms, gather evidence, understand business impact and escalate issues when they exceed my responsibilities. Defensive security adds another layer: thinking about how technical weaknesses could be exploited and which controls can reduce the risk.

The room also reinforced that good security does not mean immediately replacing every system with a reported issue. Effective decisions involve asset visibility, investigation, appropriate remediation and verification that the change actually addressed the weakness.

## Key takeaways

1. System compromise can occur independently of direct user interaction.
2. Vulnerabilities, misconfigurations and supply-chain weaknesses require different types of analysis.
3. CVE identifies a published vulnerability; CVSS helps score severity but does not replace a full risk assessment.
4. Patching, hardening, access controls and monitoring work together as defence in depth.
5. Remediation should be tested and verified, with appropriate documentation and escalation.

## Next steps

I want to develop my understanding of vulnerability management, secure configurations and how SOC analysts detect signs that a system weakness may have been exploited. These areas will complement my Cyber Security degree, networking foundations and practical IT experience.

---

*This document reflects my own learning. It does not contain TryHackMe task answers, flags, room screenshots or a step-by-step walkthrough.*
