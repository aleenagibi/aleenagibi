<div align="center">

# Aleena Gibi

**Data Science & AI · AI Engineering · Building systems end-to-end — retrieval, NLP, backend, frontend, deployment**

<a href="mailto:aleenagibi2005@gmail.com"><img src="https://cdn.simpleicons.org/gmail/EA4335" width="30" alt="Email"></a>
    <a href="https://www.linkedin.com/in/aleenagibi2005/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linkedin/linkedin-original.svg" width="30" alt="LinkedIn"></a>
    <a href="https://github.com/aleenagibi"><img src="https://cdn.simpleicons.org/github/FFFFFF" width="30" alt="GitHub"></a>
    <a href="https://huggingface.co/Al7929"><img src="https://cdn.simpleicons.org/huggingface/FFD21E" width="30" alt="Hugging Face"></a>

</div>

<br/>

## About

Final-year **B.Sc. (Hons.) Data Science & AI** student at **CHRIST (Deemed to be University), Delhi NCR**, building AI and software systems across retrieval, NLP, backend architecture, frontend engineering, and deployment.

Previously a **6-month Frontend Developer Intern at Entab Infotech**, where repeatedly rebuilding similar school websites led to the idea behind my **School Template Engine**.

🏆 **Best Paper Award — ICEIBT 2026** for research on layered defenses against adversarial attacks on LLMs.

Currently building **GreenLens**, an agentic, carbon-aware LLM routing system as my capstone project.

<br/>

## Skills

| Area                       | Technologies                                                       |
| -------------------------- | ------------------------------------------------------------------ |
| **Languages**              | Python, TypeScript, JavaScript, R, SQL                             |
| **ML / NLP**               | PyTorch, scikit-learn, spaCy, Sentence-Transformers, Hugging Face  |
| **Retrieval / AI Systems** | FAISS, TF-IDF, Dense Retrieval, RAG, LLM Routing                   |
| **Backend**                | FastAPI, Flask, SQLAlchemy, Alembic                                |
| **Frontend**               | React, Tailwind CSS                                                |
| **Databases**              | PostgreSQL, MySQL, SQLite                                          |
| **Graphs / Algorithms**    | NetworkX, Graph Algorithms                                         |
| **Security / Systems**     | AWS, HMAC-SHA256, Chrome Extensions, Manifest V3, Blockchain / PoA |
| **Deployment / Tooling**   | Docker, Vercel, Hugging Face Spaces, Git, GitHub Actions, VS Code  |

<br/>

## Featured Projects

### 🚀 [Ripple — Business Change Intelligence](https://github.com/aleenagibi/ripple-business-change-intelligence)

`FastAPI` `PostgreSQL` `React` `TypeScript` `FAISS` `spaCy` `NetworkX`

**Enterprise AI system for analysing the downstream impact of changing business requirements.**

Ripple answers a practical question: **when a business requirement changes, what else could be affected?**

It combines **TF-IDF lexical retrieval** with **dense semantic retrieval** using Sentence-Transformers and FAISS, allowing the system to capture both exact terminology—such as API names and error codes—and semantically related content expressed differently.

Extracted business entities and relationships are used to construct a **knowledge graph with NetworkX**, allowing Ripple to surface indirect dependencies across documents, workflows, APIs, policies, and other business concepts.

The backend follows a layered **FastAPI architecture** with services, engines, repositories, and PostgreSQL persistence. The React/TypeScript frontend is deployed on Vercel, with the NLP backend deployed through Hugging Face Spaces.

**[Live Demo →](https://ripple-business-change-intelligence.vercel.app/)**

---

### 🚧 [GreenLens — Carbon-Aware LLM Routing](https://github.com/aleenagibi/GreenLens)

`Python` `LLM Routing` `FAISS` `Sentence-Transformers` `Ollama` `vLLM`

**In progress · Final-year capstone project**

An agentic inference orchestrator designed to route each task to an appropriate LLM while considering **capability, task complexity, inference cost, and carbon impact**.

GreenLens embeds incoming tasks, evaluates candidate models and deployments, and selects the smallest model on a suitable low-carbon deployment that satisfies the task constraints. The system is designed around self-hosted inference using **Ollama/vLLM**, semantic task embeddings, and live grid-carbon information.

---

### 🧠 [Cross-Phase Defense Framework](https://github.com/aleenagibi/cross-phase-defense-framework)

`DistilBERT` `GPT-2` `FGSM` `PGD` `DeepFool`

🏆 **Best Paper Award — ICEIBT Conference 2026**

A multi-layer defense framework for adversarial attacks on language models.

Instead of relying on a single defense mechanism, the framework applies protection across multiple stages:

**Data sanitization → adversarial training → runtime backdoor detection**

The prototype was evaluated on **DistilBERT and GPT-2**, using simulated data-poisoning and backdoor attacks and benchmarking against **FGSM, PGD, and DeepFool** on the IMDB and AG News datasets.

*Research paper under review for WoS publication.*

---

### 🔧 [School Template Engine](https://github.com/aleenagibi/school-template-engine)

`FastAPI` `React` `FAISS` `Sentence-Transformers` `Babel` `Docker`

An internal-tool-inspired system for finding and safely reusing components across large collections of React codebases.

Instead of searching by filename, components are indexed by **semantic meaning** using Sentence-Transformers and FAISS. A component can therefore be discovered through what it does rather than what it happens to be named.

The system also handles the harder part of reuse: merging components without introducing CSS collisions or invalid JSX. It uses **CSS scoping and an AST-based JSX merger built with Babel**, rather than regex-based manipulation or generative merging.

**[Live Demo →](https://school-template-engine.vercel.app/)**


---

### 🛡️ [FileGuard](https://github.com/aleenagibi/FileGuard)

`JavaScript` `Chrome Extension` `Manifest V3` `VirusTotal`

A Chrome extension that allows Gmail attachments to be checked against VirusTotal **before download**.

FileGuard injects inline scan controls into Gmail using `MutationObserver`, hashes attachments client-side using **SHA-256**, and sends the hash for analysis rather than automatically uploading the file. A rate-limiting queue and batch **Scan All** workflow handle VirusTotal API constraints and multi-attachment emails.

---

### 🤖 [Hybrid AI Chatbot](https://github.com/aleenagibi/hybrid-ai-chatbot)

`Python` `RAG` `LLM` `Embeddings`

A chatbot architecture built around **routing rather than blindly sending every query through RAG**.

For each query, the routing layer determines whether to use retrieved context, call an external API for information requiring current or exact data, or delegate to a specialized module.

The architecture is designed so additional tools and data sources can be added at the routing layer without retraining the underlying model.

---

### 📈 [Stock Volatility Prediction](https://github.com/aleenagibi/stock-volatility-prediction)

`Python` `Machine Learning`

An end-to-end machine-learning application that predicts a stock's near-future volatility category—**Low, Medium, or High**—using historical market data and engineered technical indicators.

---

### 🔐 [Blockchain-Based Voting System](https://github.com/aleenagibi/Blockchain-Based-Voting-System)

`Python` `Flask` `SQLite` `HMAC-SHA256` `Chart.js`

A blockchain-based voting system designed around two requirements: **auditability and voter anonymity**.

A Proof-of-Authority chain uses a configurable validator quorum, while a one-time voting-coin model separates the voter's identity from the token recorded on the ledger. The underlying data model enforces one-vote-per-person rather than relying solely on frontend restrictions.

---

### ☁️ [HoneyTrap](https://github.com/aleenagibi/HoneyTrap)

`Python` `scikit-learn` `AWS` `Random Forest`

An ML-based honeypot-traffic classification system that engineers features from AWS honeypot telemetry and uses a Random Forest classifier to distinguish benign activity from malicious traffic, achieving **over 91% accuracy**.

---

**More projects:** [Campus Path Finder](https://github.com/aleenagibi/Campus_Path_Finder) · [Verity-AI-Fake-News-Detector]([https://github.com/aleenagibi/leetcode-solutions](https://github.com/aleenagibi/Verity-AI-Fake-News-Detector) · [Full Repository List →](https://github.com/aleenagibi?tab=repositories)

<br/>

## Experience

### Frontend Developer Intern — Entab Infotech

**Dec 2025 – Jun 2026 · Delhi**

* Built and maintained frontend pages for school websites using modern web technologies.
* Developed multiple landing pages and reusable inner-page components across school projects.
* Worked within a repeated website architecture, identifying opportunities for component reuse and faster development.
* This experience directly motivated the **School Template Engine**, which turns component discovery and reuse into a searchable workflow.

<br/>

## Research

### Cross-Phase Defense Framework for Adversarial Attacks on Large Language Models

🏆 **Best Paper Award — ICEIBT Conference 2026**
*Under review for WoS publication*

Research on a layered defense strategy for adversarial attacks across the LLM pipeline, combining data sanitization, adversarial training, and runtime backdoor detection.

**Focus:** LLM security · adversarial ML · data poisoning · backdoor attacks · robustness evaluation

<br/>

## What I'm Building

**GreenLens** is currently my main focus: an agentic, carbon-aware LLM inference orchestrator exploring how model selection can account for both **task requirements and environmental cost**.

The project is also forming the basis of a second research paper.

<br/>

## Connect

<div align="center">

**Let's build something useful.**

[Email](mailto:aleenagibi2005@gmail.com) ·
[LinkedIn](https://www.linkedin.com/in/aleenagibi2005/) ·
[GitHub](https://github.com/aleenagibi) ·
[Hugging Face](https://huggingface.co/Al7929)

</div>
