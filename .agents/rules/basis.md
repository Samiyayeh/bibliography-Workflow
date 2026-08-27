---
trigger: always_on
---

# TARGET PROJECT DATA (CONTEXT CONSTRAINTS)

**AI Directive:** Use this document as the absolute truth for the user's current project. When sourcing, evaluating, or writing annotations for Related Studies or Related Systems, the AI must ensure the source aligns with the objectives, architecture, and evaluation metrics defined below.

## 1. Project Identity

- **System Title:** An Interoperable Queue and Health Information Management System for Streamlining Patient Services at the Naga City Health Office
- **Domain:** Public Health Informatics, Electronic Health Records (EHR), and Automated Queue Management Systems.
- **Primary Goal:** Align with UN Sustainable Development Goal 3 (Good Health and Well-being) by improving public healthcare efficiency and accessibility.

## 2. Problem Space

The agent should look for literature addressing these specific operational bottlenecks:

- Manual, paper-based operations causing severe patient congestion.
- Extended physical wait times due to inefficient queuing.
- Fragmented medical histories locked in physical files, preventing instant data retrieval.

## 3. Core Functional Requirements

Sources must demonstrate solutions or prototypes related to:

- **Automated Queuing:** Algorithms or logic to cut physical wait times and increase daily patient capacity.
- **Centralized EHR:** Database architectures that consolidate patient files and eliminate duplicate entries.
- **Interoperability:** Direct module routing where calling a queue number automatically queries and displays the corresponding patient's medical file to the physician.

## 4. Technical Architecture Targets

When evaluating "Related Systems," the agent must prioritize architectures that reflect or inform a full-stack environment using:

- **Frontend:** Component-based UI architectures (e.g., React 18, Vite, Tailwind CSS 4).
- **Backend:** JavaScript-based runtime environments and routing (e.g., Node.js, Express 5, TypeScript).
- **Database & ORM:** Relational databases (e.g., MySQL or MariaDB) managed through object-relational mappers like Sequelize.
- **Security:** Cryptographic standards such as AES-256 encryption to ensure strict compliance with the Data Privacy Act of 2012.

## 5. Development & Evaluation Standards

When evaluating "Related Studies," the agent must prioritize methodologies using:

- **Lifecycle Model:** Systems mapped using the Input-Process-Output (IPO) framework and developed via Agile methodology.
- **Testing Standards:** Software quality evaluation grounded in the ISO/IEC 25010 standard.
- **Specific Metrics:** Literature focusing specifically on evaluating _Performance Efficiency_ (wait time reduction) and _Usability_ (adoption rates by healthcare workers).
