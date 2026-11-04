# SOC Level 1 — Humans as Attack Vectors

**Platform:** TryHackMe  
**Learning path:** SOC Level 1  
**Topic:** Humans as Attack Vectors  
**Completed:** November 2026  
**Format:** Personal learning reflection (non-spoiler)

## Overview

This room explored how attackers exploit human behaviour, trust and everyday working practices. Although I was already familiar with phishing through my Cyber Security degree and IT support role, the exercise reinforced that defending an organisation involves **people, processes and technology**, not just technical controls.

My main takeaway is that even security-aware people can make mistakes. A successful defence should reduce the likelihood of those mistakes *and* limit the impact when they happen.

## Threats and techniques explored

| Threat | What it means for defenders |
| --- | --- |
| Phishing and impersonation | Suspicious requests may attempt to steal credentials, obtain sensitive information or convince staff to take unsafe actions. |
| Malicious links and attachments | Content that appears routine can lead to credential exposure or malware infection. |
| Social engineering | Attackers exploit urgency, authority, curiosity or familiarity to influence decisions. |
| Deepfakes and synthetic media | Audio and video can be manipulated, making independent verification increasingly important. |
| Physical and insider threats | Removable media, unauthorised access and misuse of legitimate privileges create risks beyond email. |

These techniques can overlap. A convincing message may combine impersonation, a malicious website and a request for authentication details.

## Defensive measures

- **Security awareness:** Teach staff how to recognise suspicious requests and how to report concerns without fear of embarrassment.
- **Email and web protection:** Use filtering, safe-link inspection and other controls to reduce exposure to known malicious content.
- **Identity and access management:** Apply appropriate authentication, least privilege and strong account-recovery procedures.
- **Endpoint detection and response (EDR):** Monitor endpoints for suspicious behaviour and support investigation or containment when needed.
- **Verification and reporting:** Confirm unusual requests through trusted channels and provide an accessible route for reporting suspected incidents.

No single control is completely reliable. Defence in depth is valuable because one missed warning should not automatically become a major incident.

## Personal reflection

I have encountered suspicious emails and identity-verification processes in my service desk work, so this topic felt particularly relevant. My experience has shown me the importance of applying procedures consistently, even when a caller or message initially appears legitimate.

An earlier phishing-awareness exercise also taught me a lesson in humility: **knowing the warning signs does not make someone immune to distraction or a convincing message**. I now view security awareness as something that should support people, rather than simply blame them for errors.

I particularly enjoyed considering how an analyst should balance caution with evidence. A strange domain, unusual attachment or unexpected request can justify investigation, but a reliable decision should consider multiple indicators and the organisation's response procedures.

## Key takeaways

1. Human-focused attacks often target trust and decision-making rather than software vulnerabilities.
2. Awareness training helps, but technical safeguards and strong identity controls remain essential.
3. Clear reporting processes help defenders respond before an incident spreads.
4. Analysts should document observations and explain their reasoning rather than assume that one indicator proves an attack.

## Next steps

As I continue SOC Level 1, I want to build practical confidence in phishing analysis, security alert triage and endpoint investigations. I also plan to keep connecting what I learn with my professional experience in identity management and incident support.

---

*This document reflects my own learning. It does not contain TryHackMe task answers, flags, room screenshots or a step-by-step walkthrough.*
