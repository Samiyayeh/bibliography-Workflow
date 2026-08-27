# [1] Bahmni Hospital Management System: Patient Queue Module

**Category:** [[Related System International]]

## ACM Citation

`[1] Bahmni Coalition. 2023. Configuring Patient Lists and Queue Workflows in Bahmni. Bahmni Coalition, Bengaluru, India. Retrieved August 26, 2026 from https://bahmni.atlassian.net/wiki/spaces/BAH/pages/32014629/Configure+Patient+Lists+Queues`

## Annotated Analysis

### Paragraph 1: System Mechanics & Limitations

Bahmni implements outpatient patient flow management through a multi-tiered architecture that integrates a React/AngularJS presentation layer, an OpenMRS Java Spring service layer, and a MySQL relational database. The queue infrastructure operates via configurable extension points defined in `extension.json`, where UI tabs execute parameter-driven SQL search handlers (`org.bahmni.patient.search`) to filter active clinic visits by triage category, provider assignment, and encounter status. Cross-service state synchronization between the electronic medical record, laboratory, and billing sub-systems relies on AtomFeed event polling. However, continuous client-side HTTP polling across distributed departmental modules introduces overhead and synchronization delays under high-concurrency outpatient traffic.

### Paragraph 2: Project Alignment & Gap Resolution

For the Naga City Health Office Health Information System (NCHO HIS), this system illustrates the structural decoupling of patient queuing configurations from core clinical record schemas. Specifically, the NCHO HIS adapts this multi-service queue routing for municipal walk-in clinics across consultation, triage, and dispensary stations. In contrast to Bahmni's multi-container AtomFeed polling mechanism, the NCHO HIS utilizes a 3-tier local intranet architecture with native WebSockets to broadcast instantaneous queue transitions directly across clinical clients. This technical choice aligns with ISO/IEC 25010 performance efficiency and functional suitability standards by eliminating physical bottlenecks and reducing manual logbook dependencies.
