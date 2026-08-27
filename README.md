# BiblioSkill: Antigravity Automated Bibliography Agent

An intelligent, rule-governed workflow and knowledge management setup designed for **Google Antigravity IDE** and **Obsidian**. This setup systematically discovers, verifies, and generates ACM-formatted annotated bibliography entries for academic research, related studies, related systems, and related literature.

---

## 📌 Project Focus & Context (`basis.md`)

This repository is calibrated around the following target capstone/research project:

- **System Title:** *An Interoperable Queue and Health Information Management System for Streamlining Patient Services at the Naga City Health Office*
- **Domain:** Public Health Informatics, Electronic Health Records (EHR), and Automated Queue Management Systems.
- **Strategic Goal:** UN Sustainable Development Goal 3 (Good Health and Well-being).
- **Core Problem Space:**
  - Manual, paper-based patient intake causing severe clinic congestion.
  - Extended physical wait times due to uncoordinated queuing.
  - Fragmented medical records preventing instant clinician retrieval.
- **Evaluation Standards:** ISO/IEC 25010 Software Quality Standards, Input-Process-Output (IPO) framework, and Agile development lifecycle.

---

## 🚀 Key Features

- **Strict Source Grounding & Zero Hallucination:** Every entry is sourced from verified peer-reviewed publications (2021–2026) with active, globally resolving DOIs/URLs.
- **Anti-AI Vocabulary & Tone Guardrails:** Strict exclusion of overused AI buzzwords, manufactured rule-of-three rhetoric, and dramatic summaries in favor of objective academic phrasing.
- **Standardized ACM Citations:** Formats bibliographic references strictly according to Association for Computing Machinery (ACM) guidelines.
- **Targeted 2-Part Annotations:**
  - **Summary:** Single-sentence distillation of the problem, methodology, and empirical findings.
  - **Relevance:** Objective third-person justification directly mapping empirical evidence to the proposed system architecture.
- **Direct Obsidian Vault Integration:** Automated synchronization and categorization into the user's active Obsidian vault via the Obsidian Model Context Protocol (MCP) server:
  - `00_AnotatedBibliography/Related-Study International/`
  - `00_AnotatedBibliography/Related-Study local/`
  - `00_AnotatedBibliography/Related-System International/`
  - `00_AnotatedBibliography/Related-System local/`
  - `00_AnotatedBibliography/Related-Literature International/`
  - `00_AnotatedBibliography/Related-Literature local/`

---

## 📂 Repository Structure

```text
biblioSkill/
├── .agents/
│   ├── rules/
│   │   └── basis.md               # Context constraints and target system specifications
│   └── workflows/
│       └── write-bibliograp.md     # Step-by-step Antigravity workflow (/write-bibliograp)
└── README.md                      # Project setup and documentation
```

---

## 🛠️ Usage & Workflow

1. **Trigger Workflow:** In the Antigravity assistant prompt, request literature sourcing (e.g., `/write-bibliograp` or *"look for a related study local"*).
2. **Automated Search & Duplicate Check:** The agent queries the local Obsidian vault to prevent duplicate sourcing, then retrieves matching real-world publications.
3. **Review & Approval:** The agent outputs a single ACM entry with exact page/section citations for user confirmation.
4. **Vault Routing:** Upon explicit approval, the agent automatically commits the note directly into the designated Obsidian vault folder.

---

## 📄 License

MIT License. Designed for academic and research workflows.
