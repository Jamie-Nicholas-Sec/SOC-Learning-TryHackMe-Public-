# Splunk: Introduction to SIEM and Log Analysis | TryHackMe SOC Level 1

**Platform:** TryHackMe  
**Pathway:** SOC Level 1  
**Room:** Splunk  
**Status:** Completed  
**Focus:** SIEM fundamentals, log ingestion, indexing and basic SPL searches

## Overview

As I work towards a career in Security Operations, learning to use a Security Information and Event Management (SIEM) platform is one of my main priorities. Splunk is a tool I have seen mentioned regularly when researching SOC roles, so I was particularly interested in getting hands-on experience with its interface.

This room introduced the main components of Splunk and guided me through importing and searching a dataset of VPN logs. It demonstrated how a large amount of raw event data can be organised and searched to answer specific investigation questions.

> **Public learning reflection:** This is a summary of the concepts and skills I practised, rather than a room walkthrough. Challenge answers, specific investigation values and task-by-task solutions have been omitted.

## Key Learning Points

### 1. Understanding Splunk's Components

I explored how log data moves through a Splunk environment:

- **Forwarder:** Collects and sends data from monitored systems to Splunk. A forwarder is designed to be lightweight, although it still uses some endpoint resources. It is not the same thing as an EDR agent.
- **Indexer:** Receives and processes incoming data, creates searchable indexes and stores events for later analysis.
- **Search & Reporting:** Provides the interface where analysts can search indexed events and examine results using Splunk Search Processing Language (SPL).

I also became more familiar with the Splunk interface, including its navigation, apps and search functionality.

### 2. Working with Different Log Sources

The room discussed how Splunk can collect data from a range of systems, including Windows and Linux hosts, web servers and databases.

For the practical exercise, I worked with **sample VPN logs**. Viewing the raw data first helped me appreciate how difficult it would be to manually locate relevant events in a large dataset.

This made the purpose of a SIEM much clearer: it provides a way to bring data into a searchable system so an analyst can find events that are relevant to an investigation.

### 3. Importing and Indexing Data

I used the Splunk lab environment to upload the supplied log file and configure it for searching.

The guided process introduced me to:

1. Selecting a data source.
2. Identifying the source type and reviewing how the data is interpreted.
3. Configuring input settings and an index.
4. Reviewing the import configuration.
5. Opening the indexed events in **Search & Reporting**.

It was useful to see the difference between looking at raw data and examining events through an indexed, searchable interface.

### 4. Introduction to SPL

I practised running **Search Processing Language (SPL)** queries provided by the room to explore the VPN dataset.

Some of the concepts introduced were:

| SPL concept | Purpose |
|---|---|
| `index` | Choose which indexed dataset to search |
| `search` | Filter events using specified conditions |
| `spath` | Extract fields from structured data such as JSON |
| `stats count` | Count events matching a search |
| `stats values()` | Summarise distinct values of a field |

These searches helped me understand how an analyst could narrow a large collection of logs to events associated with a particular user, address or location without manually reading every entry.

**An important distinction:** The room supplied the commands, and I followed the guided exercises. I am not claiming to be able to write complex SPL independently yet. Learning to construct and adapt my own searches is the next step.

## Personal Reflection

This was one of the rooms I had been looking forward to most because of my interest in becoming a junior SOC analyst.

I particularly liked seeing how Splunk could turn a large, difficult-to-read dataset into something an analyst could investigate. My best comparison is **finding a needle in a haystack**: raw logs contain a huge amount of information, but searchable fields and targeted queries help locate the part that matters.

Although I was mostly copying the supplied SPL queries, that still gave me valuable exposure to the workflow and helped me become more comfortable navigating the platform. I now have a much clearer idea of what importing data, creating an index and searching events actually looks like.

I also see an overlap with my current work as an **IT Service Desk Analyst**. In both environments, the goal is to gather information, narrow down a problem and document findings. The difference in SOC work is that the evidence often comes from security telemetry and log analysis.

## Skills Practised

- Navigating the Splunk interface and Search & Reporting app.
- Understanding the roles of forwarders and indexers.
- Importing sample VPN log data.
- Configuring an index and reviewing ingested events.
- Running introductory SPL searches.
- Filtering and summarising event data.
- Interpreting how log searches support SOC investigations.

## What I Want to Learn Next

My next objective is to progress from **running guided queries** to **building and explaining simple queries independently**. I would like to practise changing search conditions, exploring event fields, comparing results and understanding why a particular search is useful during alert triage.

## Conclusion

Completing this room gave me a practical introduction to Splunk and reinforced why SIEM skills are relevant to the SOC career path I want to pursue.

I am still at the beginning of learning SPL, but I enjoyed this exercise and feel more confident approaching future log-analysis rooms.

---

*This write-up is my own learning reflection. It intentionally excludes TryHackMe flags, room answers and challenge-specific solutions.*
