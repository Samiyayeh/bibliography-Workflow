# BiblioSkill: Antigravity Automated Bibliography & Obsidian Knowledge Graph

An automated academic research workflow and knowledge management engine designed for **Google Antigravity IDE** and **Obsidian**. This repository integrates AI agent workflows with Obsidian via the Model Context Protocol (MCP) to systematically discover, verify, cite, annotate, and link academic studies, software systems, and literature for research projects.

---

## 📌 Project Focus & Context (`basis.md`)

This repository is calibrated around the following target capstone/research project:

- **System Title:** *An Interoperable Queue and Health Information Management System for Streamlining Patient Services at the Naga City Health Office*
- **Domain:** Public Health Informatics, Electronic Health Records (EHR), and Automated Queue Management Systems.
- **Strategic Goal:** UN Sustainable Development Goal 3 (Good Health and Well-being).
- **Core Problem Space:** Manual paper-based intake, extended physical waiting times, and fragmented clinical records.
- **Evaluation Standards:** ISO/IEC 25010 Software Quality Standards, Input-Process-Output (IPO) framework, and Agile development lifecycle.

---

## 🚀 Key Capabilities

- **Zero-Hallucination & Live Verification:** Sourced exclusively from real, peer-reviewed publications (2021–2026) with globally resolving DOIs/URLs.
- **Anti-AI Jargon Guardrails:** Strict exclusion of overused AI buzzwords (*delve, testament, paramount, seamless, robust, pivotal, fostering, game-changer, moreover, furthermore*) in favor of objective academic phrasing.
- **Standardized ACM Citations:** Formats references strictly according to the Association for Computing Machinery (ACM) guidelines.
- **Targeted 2-Part Annotations:** Single-sentence summary + strict third-person relevance linking empirical evidence to the target project architecture.
- **Obsidian Graph View Linking:** Automatically generates bidirectional wikilinks to construct a clean hierarchical graph network:
  `[[Bibliography]]` ➔ `[[Category Hub]]` ➔ `[[Individual Entry]]`
- **Single-Vault Architecture:** Your live Obsidian vault is the direct Git repository—no duplicate copying needed.

---

## ⚙️ Setup & Installation Guide

Follow these steps to set up the workflow from scratch on a new machine or environment:

### Step 1: Clone the Repository as an Obsidian Vault
Clone this repository directly to your local computer:
```bash
git clone https://github.com/Samiyayeh/bibliography-Workflow.git
```

### Step 2: Open Vault in Obsidian
1. Open **Obsidian**.
2. Click **Open folder as vault**.
3. Select the cloned `bibliography-Workflow` (or `Bib`) directory.
4. Open **Graph view** (`Ctrl + G`) to see your interactive bibliography network.

### Step 3: Configure Obsidian MCP Server in Antigravity IDE
To allow Antigravity to create and link notes directly in your Obsidian vault, ensure the Obsidian MCP server is configured in your Antigravity configuration (`~/.gemini/antigravity-ide/mcp_config.json` or `mcp_config.json`):

```json
{
  "mcpServers": {
    "obsidian": {
      "command": "npx",
      "args": [
        "-y",
        "@modelcontextprotocol/server-obsidian",
        "C:\\path\\to\\your\\vault"
      ]
    }
  }
}
```
*(Replace `C:\\path\\to\\your\\vault` with your actual vault directory path).*

### Step 4: Customize Your Project Context (Optional)
If adapting this workflow for a different capstone or research paper:
1. Open `.agents/rules/basis.md`.
2. Edit the **Project Identity**, **Problem Space**, **Technical Architecture**, and **Evaluation Metrics** to match your project specifications.
3. The AI agent will automatically align all future annotations with your updated criteria.

---

## 🛠️ How to Use in Antigravity IDE

Once set up, interact with Antigravity using simple natural language prompts:

### 1. Triggering Sourcing in Chat
Type any of the following commands in the Antigravity prompt:
- `"Look for a related study local"`
- `"Search for another related study international"`
- `"Find a related literature local"`
- `"Look for a related system international"`

### 2. Review & Approval Flow
1. **Candidate Presentation:** Antigravity presents a single candidate entry with:
   - Full ACM Citation (with direct active URL)
   - 1-Sentence Summary
   - 3rd-Person Relevance
   - Exact Source References & Direct Quotes
2. **Approval:** Reply with `"approve"` or `"disapprove"`.
3. **Automated Vault & Graph Integration:** Upon approval, Antigravity automatically:
   - Writes the Markdown note into the corresponding folder (e.g., `00_AnotatedBibliography/Related-Study local/`).
   - Inserts `**Category:** [[<Category Hub>]]` at the top of the note.
   - Appends `[[<New Entry>]]` to the Category Hub note, keeping your Obsidian Graph View connected.

---

## 📂 Vault & Graph View Structure

```text
├── Bibliography.md                                # Master Hub Note
├── 00_AnotatedBibliography/
│   ├── Bibliography.md
│   ├── Related-Study International/              # International empirical studies
│   │   ├── Related Study International.md         # Category Hub
│   │   └── [Individual Study Notes].md
│   ├── Related-Study local/                      # Philippine empirical studies
│   │   ├── Related Study local.md                 # Category Hub
│   │   └── [Individual Study Notes].md
│   ├── Related-Literature local/                  # Local policies, reviews, and frameworks
│   │   ├── Related Literature local.md            # Category Hub
│   │   └── [Individual Literature Notes].md
│   ├── Related-Literature international/          # International reviews and guidelines
│   │   └── Related Literature international.md    # Category Hub
│   ├── Related-System International/             # International health software architectures
│   │   ├── Related System International.md        # Category Hub
│   │   └── [Individual System Notes].md
│   └── Related-System local/                     # Philippine health systems & prototypes
│       └── Related System local.md                # Category Hub
├── .agents/
│   ├── rules/basis.md                             # Context constraints & ground truth
│   └── workflows/write-bibliograp.md              # Workflow step-by-step instructions
└── README.md
```

---

## 🔄 Synchronizing with GitHub

Since the vault is a Git repository, backup your notes anytime:
```bash
git add .
git commit -m "feat: add new annotated studies and graph links"
git push origin main
```

---

## 📄 License

MIT License. Designed for academic research, health informatics, and computer science capstone projects.
