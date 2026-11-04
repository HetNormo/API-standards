---
layout: doc-draft
---

# EDA Principles & Guidelines

| <!-- -->             | <!-- -->   |
| :------------------- | :--------- |
| __Version__              | 0.4    |
| __Status__               | Concept    |
| __Publication date__     | 2026-09-02 |
{: .header-table }

This document is a publication of Het Normo. In the pursuit of completeness and correctness of data, we kindly request you to submit comments, additions and improvements regarding this document by [raising a ticket]({{ site.github.issues_url }}) in this repository. 

## Document annotations

Please find the following information here:

[Changes](changes.md) - for all changes in this publication\
[Signoffs](signoffs.md) - for notification and signoffs for publication\
[References](../references.md) - for references to other publications\
[Dictionary](../dictionary.md) - explanatory guide for terms and abbreviations

## Table of contents

* Do not remove this line (it will not be displayed)
{:toc}

## Referenced appendices

* [Decision Tree: State Transfer versus Notification](../attachments/eda-decision-tree.md)
<!-- * [HTTP operation usage](../attachments/Use-of-HTTP-operations-for-RESTful-APIs.html) -->

## Introduction

Event-Driven Architecture (EDA) is a proven pattern for efficient data exchange in distributed systems. In the energy sector, it brings clear benefits: when a register or asset changes - for example, an update to the primary part of a metering installation - producers publish events so market participants can react immediately without continuous querying. This reduces latency and network load, eliminates tight coupling between systems, and allows components to scale independently. These properties make EDA especially well suited to handle meter changes, price fluctuations and other real-time events that require coordinated action across many energy-market participants.

This specification defines principles and guidelines to standardize event-driven design within the Dutch energy sector. It was developed by the API Strategy Working Group on behalf of Het Normo (TE005), and builds on the Community of Practice Secure Architecture (CoP SA) *Vision Document on Event-Driven Architecture*.

### Alignment with broader initiatives
This document reflects and consolidates lessons from both energy-sector practice and public-sector initiatives:
*	The CoP SA Vision Document (2024)[^1] identified EDA as a key pattern for the energy domain and recommended concrete guidance - which this specification supplies.
*	The Dutch government's Notification Services Project (2022)[^2], conducted by VNG Realisatie for the Ministry of the Interior and Kingdom Relations, established standards for automated notifications within government applications and promoted event-driven working methods across public sector organizations.

Through collaboration with the API Knowledge Platform[^3] - a public initiative promoting cooperation among government parties working with APIs and standards - this document incorporates lessons learned from both energy sector experience and broader government implementation efforts such as the Notification Services Project.

### Principles and guidelines
This document pairs strategic principles with actionable guidelines:
*	Principles state the core values and strategic intent behind adopting EDA.
*	Guidelines translate those principles into concrete implementation steps and recommendations.
Together they ensure architectural decisions are both conceptually sound and readily applied in practice.

### Document objective
This specification provides a consistent, business-driven, event-centric framework for implementing EDA in the energy sector. Its principles and guidelines capture industry best practices to promote interoperable, scalable architectures that respond effectively to domain events while maintaining robustness and long-term evolvability across the sector.


[^1]: Referred documents can be found in the global [document reference](../references.md).
[^2]: Referred documents can be found in the global [document reference](../references.md).
[^3]: Referred documents can be found in the global [document reference](../references.md).

<!-- ## Design rules

The STD rules are the standards set by other bodies that guide the APIs designed and developed by the energy sector.

The remainder of the document contains the guidelines that have been drawn up based on best practices and lessons learned and are guiding for the APIs that are designed and developed by the energy sector. These guidelines are supplementary and/or prevailing to the API strategy for the Dutch government (ASNO). -->

