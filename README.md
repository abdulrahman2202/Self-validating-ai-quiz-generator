# Agentic AI Quant Problem Generator

An **Agentic AI system** that autonomously generates quantitative word problems, validates them using dual solver agents, and produces verified quiz-ready questions.
The system uses **workflow orchestration with N8N** and **Gemini AI models** to ensure mathematical correctness and reduce hallucinations.

---

## 🚀 Overview

Traditional AI problem generators may produce incorrect or logically inconsistent questions.
This project solves that by implementing a **multi-agent validation pipeline** that verifies every generated problem before it is accepted.

The system uses multiple specialized AI agents:

* **Research Agent** – gathers context and mathematical problem patterns
* **Problem Generation Agent** – generates quantitative word problems
* **Solver Agents (Dual Validation)** – independently solve the generated problem
* **Orchestration Agent** – coordinates the workflow and rejects inconsistent outputs

Only questions that pass validation are exported as final quiz content.

---

## 🧠 Key Features

* Multi-agent AI architecture
* Autonomous quantitative word-problem generation
* Dual-agent solver validation to detect incorrect outputs
* Hallucination rejection mechanism
* Automated quiz generation pipeline
* Accuracy reporting for generated questions
* Workflow automation using N8N
* Gemini AI model integration

---

## 🏗 System Architecture

```
User Request
      │
      ▼
Research Agent
      │
      ▼
Problem Generator Agent
      │
      ▼
Dual Solver Agents
      │
      ├── If answers match → Valid
      └── If answers mismatch → Reject
      │
      ▼
Quiz Generator
```

---

## ⚙️ Tech Stack

**AI & LLM**

* Gemini AI

**Automation**

* N8N Workflow Automation

**Core Concepts**

* Agentic AI Systems
* Multi-Agent Architecture
* Prompt Engineering
* AI Output Validation
* Hallucination Detection

---

## 📂 Project Structure

```
agentic-ai-quant-problem-generator
│
├── agents
│   ├── research_agent
│   ├── problem_generator
│   ├── solver_agent
│
├── workflows
│   ├── n8n_pipeline.json
│
├── prompts
│
├── evaluation
│
└── README.md
```

---

## 🔧 Workflow

1. User requests a set of quantitative problems.
2. Research agent gathers patterns and problem templates.
3. Problem generation agent creates new questions.
4. Two independent solver agents solve the question.
5. Results are compared.
6. If answers match → question is accepted.
7. If answers differ → question is rejected.

---

## 📊 Example Output

```
Question:
A train travels 60 km in 1 hour. How far will it travel in 4 hours?

Answer:
240 km

Validation Status:
✔ Verified by dual solver agents
```

---

## 🎯 Use Cases

* Educational quiz generation
* Math practice platforms
* AI-based tutoring systems
* Automated assessment systems
* EdTech AI tools

---


## ⭐ Support

If you find this project useful:

* Star the repository
* Share it with others
* Contribute improvements

---

##Output Image

<img width="1526" height="538" alt="Screenshot 2026-03-05 200844" src="https://github.com/user-attachments/assets/33e1e7aa-3234-417f-b923-091cfa99b368" />

