# SOC Level 1 - Elastic Stack (ELK) | TryHackMe

**Platform:** TryHackMe  
**Pathway:** SOC Level 1  
**Room:** Elastic Stack  
**Status:** Completed  
**Focus:** SIEM fundamentals, VPN log analysis, filtering, queries, and dashboards

## Overview

In this room, I explored the **Elastic Stack (ELK)** and how a Security Operations Centre (SOC) can use it to collect, search, analyse, and visualise large volumes of log data.

Having recently completed an introductory Splunk room, I was interested in comparing another platform commonly used for security monitoring. This was a longer room with several practical exercises, and I particularly enjoyed the investigative side: narrowing down large datasets to find information that mattered.

## What I Learned

### 1. The Elastic Stack components

The room introduced the main parts of the stack and their roles:

| Component | Purpose |
| --- | --- |
| **Beats** | Lightweight data shippers that collect specific kinds of endpoint or service telemetry. |
| **Logstash** | Ingests and processes data, applying filters and transformations before forwarding it to a destination. |
| **Elasticsearch** | Indexes and stores data so it can be searched and analysed. |
| **Kibana** | Provides the interface for exploring events, creating visualisations, and building dashboards. |

I found it helpful to think of this as a workflow: **collect data -> process and index it -> investigate and visualise it**. The exact pipeline can vary; data does not always need to pass through every component.

### 2. Exploring VPN logs in Kibana

The practical tasks used a supplied dataset of VPN connection events. Working in **Kibana Discover**, I became more comfortable with:

- Choosing the relevant data view for the logs being investigated.
- Setting an appropriate **time range** before interpreting search results.
- Inspecting event fields, including users, source addresses and connection activity.
- Applying field-based filters to narrow the results.
- Using the event timeline to spot changes or spikes in activity.

It became clear why an analyst needs to understand the scope of a search before drawing conclusions from its results.

### 3. Searching and combining filters

I practised progressively narrowing searches using field values and logical operators such as **AND**, **OR**, and **NOT**. I also explored wildcard searches and date-based conditions.

This helped me understand the difference between looking at all available events and asking a specific investigative question, such as whether a particular account showed unusual login activity during a defined period.

One area I want to keep practising is **query structure**, especially ensuring that combinations of conditions return the events I actually intended to include. When results looked inconsistent, I had to reconsider the filters and time settings rather than assuming the initial output was correct.

### 4. Visualisations and dashboards

I also worked with Kibana's visualisation features, selecting fields and presenting summaries of log activity in a more readable way.

I practised saving visualisations and adding them to a dashboard. This showed me why dashboards can help an analyst identify patterns quickly, while still needing to inspect the underlying events for context.

## Challenges and Lessons Learned

The most useful lesson came from a mistake: I initially received an unexpected result because my **time filter was too narrow**. After reviewing the selected period and expanding it, the results made more sense.

I also encountered search results that did not initially match my expectations. Rather than just moving on, I experimented with the filters and tried to understand what the search was actually returning.

My main takeaways were:

- **Time ranges matter.** A technically correct filter can still miss important activity if the selected period is wrong.
- **Event counts need context.** A spike or high number of connections is a starting point for investigation, not proof of malicious behaviour.
- **Queries need checking.** Logical operators and field names can change which records appear in the results.
- **Visualisations support analysis.** They make patterns easier to spot, but do not replace examining raw logs.

## Personal Reflection

This room was one of the most enjoyable practical exercises I've completed on the SOC Level 1 pathway so far.

In the previous Splunk room, many of the searches were guided. Here, I felt more confident experimenting with filters, creating queries, investigating the results, and correcting mistakes. I am still learning the tools, but I can see progress in how I approach unfamiliar data.

As an IT Service Desk Analyst, I'm already used to gathering information, narrowing down possible causes, and documenting what I find. This exercise helped me see how those habits transfer into security monitoring, where the focus is on understanding events and deciding what deserves further investigation.

More than anything, I enjoyed the analytical process. Working through the logs reinforced my interest in pursuing a **Blue Team / SOC analyst** role in the future.

## Skills Practised

- Elastic Stack architecture and component roles
- Kibana Discover navigation
- VPN log exploration and event analysis
- Field-based filtering and time-range selection
- Basic logical search expressions
- Identifying patterns and investigating unexpected results
- Creating and saving visualisations and dashboards
- Troubleshooting my own investigative approach

## Next Steps

I want to keep practising both Elastic and Splunk, focusing on building searches with less guidance and explaining what the results do - and do not - tell me. As I continue the SOC Level 1 pathway, I'll also explore how SIEM investigation connects with alert triage and security response workflows.

---

*This is a personal learning reflection. Specific TryHackMe answers, flags, usernames, IP addresses, and step-by-step challenge solutions have been intentionally omitted.*
