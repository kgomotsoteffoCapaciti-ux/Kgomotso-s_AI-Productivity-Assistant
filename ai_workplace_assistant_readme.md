# AI Workplace Assistant 🚀

An intelligent, prompt-engineered workplace automation tool designed to eliminate administrative drag and boost daily productivity for teams, operations leads, and knowledge workers.

🔗 **Live Application:** [https://efficient-effort.lovable.app](https://efficient-effort.lovable.app)  
👤 **Author / Lead:** Kgomotso Teffo

---

## 📌 Table of Contents
- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [System Architecture](#system-architecture)
- [Prompt Engineering Strategy](#prompt-engineering-strategy)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Roadmap](#roadmap)
- [License & Contact](#license--contact)

---

## 📖 Project Overview

Knowledge workers spend between 25% and 35% of their working hours on low-value operational chores: drafting repetitive status emails, parsing noisy meeting transcripts, and manually building project checklists. 

The **AI Workplace Assistant** addresses these bottlenecks through three integrated, deterministic AI modules:
1. **Smart Email Generator:** Fast, context-aware correspondence calibrated by tone, recipient persona, and urgency.
2. **Meeting Summarizer & Decision Extractor:** Strips conversation clutter to produce actionable decision registries and task matrices.
3. **Task Planner & Work Breakdown Generator:** Uses step-by-step reasoning to transform high-level goals into chronological, dependency-aware task packages.

---

## ✨ Key Features

### 1. Smart Email Generation
- **Persona Conditioning:** Tailor messages for executives, cross-functional peers, clients, or vendors.
- **Negative Constraints:** Enforces clear, professional business language with zero generic email filler (e.g., *"I hope this email finds you well"*).
- **Action-Oriented Outputs:** Produces a clear subject line, concise body copy (under 3 paragraphs), and explicit call-to-action (CTA) deadlines.

### 2. Meeting Summarization & Decision Extraction
- **Noise Reduction:** Filters out small talk and digressions from unformatted notes or transcripts.
- **Decision Registry:** Catalogs immutable team agreements and strategic decisions.
- **Action Matrix:** Automatically formats assignees, task descriptions, and hard deadlines into clear tables or structured lists.

### 3. Task Planning & Decomposition
- **Chain-of-Thought (CoT) Breakdown:** Identifies prerequisites and dependencies before estimating effort.
- **Milestone Sequencing:** Breaks broad goals into phases (Inception, Build, Validation, Deployment).
- **JSON & Markdown Export:** Clean schemas ready for copy-pasting into Jira, Trello, or Notion.

---

## 🏗️ System Architecture

```text
[User Input]
   │
   ├──► Email: Persona + Talking Points + Tone
   ├──► Meeting: Raw Transcript / Rough Notes
   └──► Task: Objective + Scope + Constraints
   │
   ▼
[Prompt Orchestration & Validation Layer]
   │ (Role Definition + Few-Shot Exemplars + Negative Constraints)
   ▼
[Frontier LLM Engine (GPT-4o / Gemini)]
   │
   ▼
[Structured Response (Markdown & JSON)]
   │
   ├──► One-Click Clipboard Copy
   ├──► Formatted Markdown Preview
   └──► Project Management JSON Schema
```

---

## 🧠 Prompt Engineering Strategy

The application emphasizes deterministic, predictable AI behaviors through targeted prompt engineering principles:

* **Few-Shot In-Context Steering:** Feeds input-output examples directly in system prompts to fix stylistic tone and eliminate corporate clichés.
* **Role-Based Task Boundaries:** Assigns explicit roles (*Executive Communications Lead*, *Agile Delivery Specialist*, *Senior Technical Project Manager*) to scope model behavior.
* **Anti-Hallucination Guardrails:** If a meeting transcript lacks a clear task owner, the model labels it `Unassigned - Needs Review` rather than inventing an assignee.
* **Strict Output Contracts:** Uses markdown tables and valid JSON formatting to ensure output consistency across repeated runs.

---

## 💻 Tech Stack

- **Frontend / Deployment:** [Lovable.app](https://efficient-effort.lovable.app) (Single Page Application, responsive layout, real-time markdown rendering)
- **Model Engine:** Multimodal Frontier LLMs (OpenAI GPT-4o / Google Gemini API)
- **Data Interoperability:** Markdown, JSON, REST API protocols
- **Styling:** Modern utility CSS, responsive mobile-first UI

---

## 🚀 Getting Started

### Access the Live Build
Visit the hosted web application directly:  
👉 **[https://efficient-effort.lovable.app](https://efficient-effort.lovable.app)**

### Using the Assistant
1. Select the desired module tab (**Smart Email**, **Meeting Summarizer**, or **Task Planner**).
2. Enter your raw inputs, select your target audience/tone, or paste your meeting transcript.
3. Click **Generate** to receive an audited, structured output.
4. Copy directly to your clipboard or export for project tracking.

---

## 🗺️ Roadmap

- [x] **Phase 1 (MVP):** Web UI live on Lovable with Email, Summarization, and Task Planning modules.
- [ ] **Phase 2:** Direct integrations via webhooks for Google Workspace (Gmail/Docs) and Slack.
- [ ] **Phase 3:** Retrieval-Augmented Generation (RAG) to allow queries against custom company SOP documents and PDFs.

---

## 📄 License & Contact

Distributed under the MIT License. See `LICENSE` for more information.

* **Author:** Kgomotso Teffo
* **Email:** [Kgomotsoteffo687@gmail.com](mailto:Kgomotsoteffo687@gmail.com)
* **Live App:** [efficient-effort.lovable.app](https://efficient-effort.lovable.app)