---
description: Step by step Of writing A BiblioGraphy
---

# RSS & RRL Annotated Bibliography Generator

**Description:** An Antigravity workflow to systematically source real literature or software systems and generate an ACM-formatted annotated bibliography entry.

## Step 1: Request Analysis & Sourcing

- Ask the user for their topic and clarify if they are looking for a "Related Study", a "Related System", or "Related Literature".
- **Vault Inspection Check:** Before searching for any external sources, you must first inspect the local Obsidian vault directories:
  - `00_anotatedbibliography/Related-Study international/` (and local)
  - `00_anotatedbibliography/Related-System international/` (and local)
  - `00_anotatedbibliography/Related-Literature international/` (and local)
- Do not recommend, select, or generate an entry for any source that already exists within these vault directories to prevent duplicate entries.
- Use search capabilities to find a **real, existing** source that matches the category and is not already in the vault.
- **CRITICAL CONSTRAINT:** Do not hallucinate sources. Verify that the study or system actually exists with a valid DOI, URL, or publication record and is freely accessible in its entirety.
- Only look for sources published between 2021–2026.

## Step 2: ACM Citation Formatting

- Format the retrieved source reference strictly using the Association for Computing Machinery (ACM) reference format.

## Step 3: Targeted 2-Part Annotation

Draft a short descriptive text (the annotation) beneath the citation. **Strict Source Grounding:** All information in the annotation MUST be extracted directly from the verified source. Do not infer, assume, or invent methodologies, features, or metrics that are not explicitly stated in the text. You must also pinpoint exactly where in the source you found this information.

- **Summary (1 Sentence):**
  - _For a Study:_ Summarize the research problem, methodology, and theoretical findings in a single sentence.
  - _For a System:_ Summarize the core technical architecture, interface, and functional features in a single sentence.
  - _For Literature:_ Summarize the core concepts, legal frameworks, or theoretical models discussed in the publication.
- **Relevance (Strictly 3rd Person):**
  - _For a Study:_ Explain how the theoretical findings and evaluated data justify the logic of the proposed project.
  - _For a System:_ Explain how the software/hardware architecture and its technical efficiency inform the development of the proposed project.
  - _For Literature:_ Explain how these theories, standards, or legal frameworks establish the foundational guidelines or constraints for the proposed system.
  - _Constraint:_ The relevance section MUST be written entirely in the **third person**. Never use "you," "your," "I," or "my." Use objective phrasing such as "the proposed system," "the current study," or "the researchers."

## Step 4: Tone and Style Constraints

You must strictly adhere to the following academic writing rules when drafting the annotation:

1. **Zero-Hallucination Rule:** Do not add external knowledge to the summary. If the source does not mention a specific framework, metric, or finding, do not include it.
2. **Banned AI Vocabulary:** NEVER use overused AI buzzwords (e.g., _delve, testament, paramount, seamless, robust, pivotal, fostering, game-changer, moreover, furthermore, beacon, cornerstone, revolutionizing_).
3. **Ban Manufactured Rhetoric:**
   - Avoid forced rule-of-three rhythm lists (e.g., "improves workflow, enhances accuracy, and optimizes throughput").
   - Avoid X-not-Y parallel constructions (e.g., "the challenge is not X, but Y"). Rewrite as direct statements.
   - Do not use dramatic, melodramatic summaries, or punchlines at paragraph endings.
4. **Academic Hedging:** Use evidence-based qualifiers (_"suggests", "indicates", "demonstrates a reduction of"_) rather than absolute claims (_"completely solves", "guarantees", "eliminates"_).
5. **Direct Transitions:** Use functional research connectors (_"However," "Specifically," "In contrast," "Conversely"_) instead of conversational filler or dramatic transitions.
6. **Technical Grounding over Vague Praise:** Replace abstract descriptive hype (e.g., "state-of-the-art platform") with specific technical specs, frameworks, or methodologies relevant to the source (e.g., _architectural patterns, database models, cryptographic standards, or specific statistical evaluation metrics_).

## Step 5: Single Entry Output & Approval

- Output exactly **one** complete bibliography entry at a time matching the structure:
  **[ACM Citation]**
  - **Summary:** [Text]
  - **Relevance:** [Text]
  - **Source Reference(s):** [List the specific page numbers, section headings (e.g., "Methodology", "Section 3.2"), or provide a brief direct quote used to ground the summary and relevance.
- Ask the user for approval or feedback on the entry. **Stop execution.** Do not generate the next entry or execute any file transfers until the user explicitly approves the current one.

## Step 6: Obsidian Vault Integration & Routing

- Upon receiving explicit user approval, automatically transfer and save the approved entry as a Markdown (`.md`) file into the local Obsidian vault.
- Determine the geographic origin of the study, system, or literature to route the file to the correct directory path:
  - For Study international sources: Save to `00_anotatedbibliography/Related-Study international/`
  - For Study local sources: Save to `00_anotatedbibliography/Related-Study local/`
  - For System international sources: Save to `00_anotatedbibliography/Related-System international/`
  - For System local sources: Save to `00_anotatedbibliography/Related-System local/`
  - For Literature international sources: Save to `00_anotatedbibliography/Related-Literature international/`
  - For Literature local sources: Save to `00_anotatedbibliography/Related-Literature local/`
- **Entry Linking:** Place the category link at the top of the new note:

  ```markdown
  **Category:** [[<Category Hub Name>]]
  ```

  - **Category Hub Linking:** Append the new note's wikilink `[[<Note Name>]]` to the corresponding category hub note (e.g., `Related Study local.md`), which connects to `[[Bibliography]]`.
  - **Graph Hierarchy Maintained:**
    `[[Bibliography]]` ➔ `[[<Category Hub>]]` ➔ `[[<Individual Entry>]]`
