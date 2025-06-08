# AI-Driven Attack Vector Tree Generation for Enhanced TARA in Automotive functions(threat_modelling)
#  Phase 2: AI-Powered Threat Modeling for Automotive Cybersecurity

This project marks **Phase 2** of our ongoing development of a dynamic threat modeling system for the automotive domain. It automates the generation and visualization of attack trees using **Large Language Models (LLMs)**, stores threat data in **MongoDB**, and maintains a structured **CSV threat library** for security analysis and decision-making.

---

##  Key features

-  Fully **automated attack tree generation** via prompt-based input.
-  **Real-time visualizations** using Mermaid.js rendered in the UI.
-  A **dynamic CSV threat library** that updates with every new prompt.
-  **Prompt-to-tree mapping** system with support for labels and aliases.
-  Seamless integration between UI ↔ LLM ↔ MongoDB.

---

  System Architecture

🔹 UI Layer
- Accepts free-form user prompts or selects from predefined labels/aliases.
- Displays Mermaid-based visual attack trees and summaries.

🔹 LLM Engine
- Converts surface + goal prompts into:
  - Attack tree structure 
  - Summary of attack paths, vectors, and methods
- Reduces manual tree creation and ensures consistency.

 🔹 MongoDB Backend
- Stores:
  - Prompts and their aliases
  - Generated attack trees and summaries
  - Versioned threat data for querying

🔹 CSV Threat Library
- Auto-updated for every new threat model
- Columns: `Attack Surface`, `Goal`, `Vectors`, `Techniques`, `Methods`, `Paths`
- Supports external analysis and portability

---


