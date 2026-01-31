# AXIS - IBM Hackathon 2026

![IBM Watsonx](https://img.shields.io/badge/Powered%20by-IBM%20watsonx-blue)
![Status](https://img.shields.io/badge/Status-Hackathon%20MVP-orange)
![Agentic AI](https://img.shields.io/badge/Focus-Agentic%20AI-green)
![Llama-3.2](https://img.shields.io/badge/Model-Llama--3.2--90b-white)

**IBM Hackathon 2026 | Challenge: Agentic AI with watsonx**

> **Axis** is not a chatbot; it is an ecosystem of autonomous agents acting as the connective tissue between static legal contracts and dynamic operational execution.

---

## 🛠️ Repository Content
This repository serves as the documentation and architecture hub for the solution:
* **/workflows**: Flowcharts of the agentic logic and skill orchestration in watsonx Orchestrate.
* **/prompts**: System prompt configurations for the Llama-3.2 model.
* **/docs**: Implementation guides and business use cases for the demo (Project timeline extends beyond February 4th, as it was developed on a continuous improvement basis).

---

## 📑 Project Overview
In today’s business environment, compliance is often a reactive and manual process. Contracts remain confined in PDF repositories, disconnected from daily billing and communication systems.

**Axis** solves this through **Agentic AI**, transforming passive clauses into active sentinels that:
1.  **Reason** about the legality of an invoice or an email.
2.  **Orchestrate** enterprise tools (Jira, Trello, Slack).
3.  **Act** proactively regarding expiration dates or compliance risks.

---

## ⚙️ Micro-Agent Architecture
We have implemented a delegation architecture to maximize precision and minimize bias:

### 1. Contract Intelligence Agent (The Reader)
* **Model:** Llama-3.2-90b-vision-instruct.
* **Function:** Vision processing of unstructured documents.
* **Output:** Structured data (JSON) containing dates, liability limits, and price adjustment formulas, always linked to a textual citation from the original document.

### 2. Compliance Reasoning Agent (The Judge)
* **Logic:** Based on the **ReAct** framework.
* **Mission:** Evaluate whether a received invoice or a commitment in an email violates the clauses extracted by the previous agent.
* **Rigorousness:** Implements a "Mandatory Evidence" protocol. If no clause supports a judgment, the agent declares itself neutral and requests human intervention.

### 3. Action Orchestrator Agent (The Executor)
* **Role:** The operational arm within **watsonx Orchestrate**.
* **Action:** Receives structured compliance decisions and translates them into API calls to Slack, Outlook, Jira, and Trello. It does not reason about law; its focus is execution integrity.

---

## 🛠️ Technological Stack
* **AI Platform:** [watsonx.ai](https://www.ibm.com/watsonx)
* **LLM/VLM Models:** Llama-3.2-90b-vision-instruct (Multimodal).
* **Orchestration:** [watsonx Orchestrate](https://www.ibm.com/products/watsonx-orchestrate) utilizing Agentic Workflows.
* **Decision Framework:** ReAct Logic (Reason, Act, Observe).
* **Integrations:** Jira Software, Slack Enterprise, Trello API, Microsoft Outlook, Google Drive.

---

## 🛡️ Guardrails and Agent Governance
Axis operates under a set of non-negotiable guidelines configured in its base behavior:

| Condition | Agentic Action |
| :--- | :--- |
| **No Hallucination** | Strict prohibition on inferring terms not present in the document. |
| **Textual Evidence** | Every compliance decision must cite the exact paragraph from the contract. |
| **Financial Safeguard** | The agent can detect invoice errors but is forbidden from executing payments. |
| **Conflict Detection** | If contradictory information is found between documents, the agent suspends action and escalates to the user. |
| **Missing Info Protocol** | Does not assume data; if a field for Jira/Trello is missing, it asks explicitly. |

---

## 🚀 Demo Flow: From Email to Action
For evaluation purposes, Axis demonstrates its autonomy through the following scenario:
1.  **Ingestion:** Receipt of a service contract via Outlook.
2.  **Reasoning:** Axis identifies a 5% annual increase and a specific start date.
3.  **Execution 1:** Automatically creates a project plan in **Trello** based on contract milestones.
4.  **Validation:** Receives an invoice showing a 10% increase.
5.  **Execution 2:** Axis detects the violation, cites the 5% increase clause, sends a **Slack** alert, and opens a dispute ticket in **Jira**.

---

## 👥 The Team
Developed for the **IBM Hackathon 2026** by:

* **[Santiago Oroz](https://www.linkedin.com/in/santiago-oroz/)** - santiago.oroz1510@gmail.com
* **[Renata Berho](https://www.linkedin.com/in/renata-berho-02264230a/)** - renaberho2@gmail.com
* **[Milagros Argañin](https://www.linkedin.com/in/milagros-arga%C3%B1in-13641a376/)** - miliarganin3@gmail.com

---
*Axis demonstrates how the power of open models in watsonx.ai transforms legal compliance into an operational advantage.*
