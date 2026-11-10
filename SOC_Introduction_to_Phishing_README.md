# Introduction to Phishing | TryHackMe SOC Level 1

**Platform:** TryHackMe  
**Pathway:** SOC Level 1  
**Room:** Introduction to Phishing  
**Environment:** Splunk-based SOC simulation  
**Status:** Completed  
**Focus:** Phishing alert triage, evidence gathering, and incident classification

## Overview

This room was my first hands-on SOC simulation using a Splunk-based environment. I entered the exercise with no previous practical experience of Splunk, so my focus was on understanding the alerts, investigating the available evidence, and making defensible classification decisions.

The scenario involved reviewing incoming email and related network security alerts, identifying potentially malicious activity, and distinguishing genuine threats from benign events. I found it challenging at first, but working through the interface and learning what information was available helped me become more confident as the simulation progressed.

## What I practised

### 1. Initial alert triage

I reviewed alerts presented in the SOC queue and looked at information such as the alert description, timestamp, sender and recipient context, email content, and associated links.

The experience reinforced that **an alert is a starting point for investigation, not proof of malicious activity**. Some events are suspicious enough to trigger detection rules but are ultimately legitimate.

### 2. Recognising phishing indicators

I considered common indicators such as:

- Messages pressuring recipients to take urgent action.
- Sender domains that impersonate familiar organisations.
- Unusual or shortened links.
- Requests to sign in or provide sensitive information.
- The relationship between the message's stated purpose and its actual destination.

These indicators need to be assessed together with additional evidence rather than treated as conclusive in isolation.

### 3. Correlating evidence

I used the available simulation tools to investigate URL reputation and considered how firewall or proxy records can help show whether a suspicious destination was accessed or blocked.

This helped me appreciate the difference between identifying a suspicious email and understanding whether further activity occurred after it was received.

### 4. Documenting decisions

I practised writing investigation notes explaining what happened, which evidence supported my assessment, and why an alert should be classified or escalated.

Clear reporting matters because another analyst may need to review or continue the investigation. A conclusion is more useful when the underlying reasoning is recorded.

## Simulation results

For my first attempt, the simulation reported:

| Measure | Result |
| --- | ---: |
| Alerts closed | 5 |
| True-positive identification rate | **100%** |
| False-positive identification rate | **50%** |
| Mean time to resolve | 9 minutes |

I successfully identified all the genuine malicious alerts, which was particularly encouraging given that this was my first time using the environment.

However, I also incorrectly classified a benign alert as malicious. This was a valuable reminder that **accurate triage involves both detecting threats and avoiding unnecessary escalations**. False positives can consume analyst time and increase pressure on a busy SOC.

## Personal reflection

What I enjoyed most was working through the investigation despite initially being unfamiliar with Splunk and the tools available in the scenario.

At first, I concentrated on the obvious details of each alert. As I explored the interface, I became more aware of the additional context and investigation features available. This changed the way I approached later alerts.

My IT Service Desk experience was useful here. I am accustomed to reviewing tickets, gathering information, documenting findings, and escalating when necessary. The SOC environment introduced a different kind of evidence and higher security stakes, but the core habits of curiosity and structured troubleshooting felt familiar.

I am pleased with the first attempt, while recognising that I can improve the quality of my written reasoning, make fuller use of available evidence, and become more confident distinguishing benign events from genuine threats.

## Skills developed

- First exposure to a Splunk-based SOC investigation environment
- Phishing indicator recognition
- Email and URL contextual analysis
- Understanding the value of firewall and proxy evidence
- True-positive and false-positive classification
- Alert reporting and evidence-based escalation
- Managing a live alert queue under time pressure

## Next steps

I plan to continue practising SIEM investigation and log analysis, learn more about Splunk searching, and improve the clarity of my incident reports. I also want to develop a more consistent approach to validating suspicious activity before reaching a final classification.

---

*This is a public reflection on my learning and simulation results. Specific scenario answers, flags, indicators, and step-by-step challenge solutions have intentionally been omitted.*
