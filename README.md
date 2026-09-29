# Prompt_Engineering_Keynote_2026

This repository contains the presentation slides and architectural documentation for the technical workshop titled **"Autonomous AI Agents and Tool Integration: From Text Completion to Autonomous Action"**, presented at the **Şarkışla Science, Art, and Culture Club**.

It covers the architectural evolution of Large Language Models (LLMs) from passive text generators to goal-oriented autonomous systems capable of reasoning, planning, and interacting with external APIs, databases, and environments.

---

## 📌 Workshop Scope & Architectural Modules

1. **Paradigm Shift (Chatbot vs. AI Agent):**
   - Contrasting passive, pre-trained parametric models with goal-driven agents that interact with external environments.
2. **Anatomy of an AI Agent:**
   - **Brain (LLM Engine):** Core reasoning, semantic parsing, and orchestration.
   - **Memory Architecture:** Short-term memory (Context Window) vs. Long-term memory (Vector Databases / RAG).
   - **Planning:** Task decomposition, iterative sub-goal generation.
   - **Tools & Actuators:** REST APIs, SQL engines, bash terminals, and environment runtimes.
3. **The Golden Rule: "Models Do Not Execute Code; They Generate Parameters":**
   - The LLM acts as an orchestrator emitting structured JSON payloads; code execution and security enforcement remain strictly on the backend.
4. **Function Calling & Tool Contracts:**
   - Defining rigid tool interfaces using JSON Schema / OpenAPI specifications and managing the end-to-end execution loop.
5. **ReAct Framework (Reason + Act):**
   - The *Thought $\rightarrow$ Act $\rightarrow$ Observation $\rightarrow$ Final Answer* cycle for grounded, evidence-based problem solving.
6. **Error Recovery & Self-Correction:**
   - Treating runtime system/API exceptions as new observations to dynamically pivot execution paths instead of failing.
7. **Guardrails & Safety Controls:**
   - Bounding agent recursion with step limits (Max Iterations).
   - Token buffers and financial thresholds (Budget Guardrails).
   - Human-in-the-Loop (HITL) approval gates for state-mutating, irreversible operations (POST/DELETE/Execute).

---

## 📁 Repository Structure

- `Otonom_AI_Agent_Mimarisi.pdf`: The minimalist, high-contrast, annotated presentation slide deck used during the session.
- `LICENSE`: MIT License.

---

## 🛠️ Session Details

- **Speaker:** Himmet Can Umutlu
- **Host Institution:** Şarkışla Science, Art, and Culture Club
- **Duration:** ~25–30 Minutes

---

## 📄 License

All documentation and presentation assets in this repository are distributed under the [MIT License](LICENSE). You are free to fork, adapt, and use this material for non-commercial educational workshops or community technical sessions.
