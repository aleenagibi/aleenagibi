<div align="center">

<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/glitch-hero.svg" width="100%" alt="Aleena Gibi — animated hero"/>

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=500&size=15&duration=2600&pause=700&color=8B949E&center=true&vCenter=true&repeat=true&width=760&lines=%24+whoami;final-year+B.Sc.+(Hons.+Research)+Data+Science+%26+AI+%40+CHRIST+Delhi+NCR;%24+tail+-f+currently.log;building+GreenLens+%E2%80%94+a+carbon-aware+LLM+inference+router" alt="typing terminal"/>

</div>

<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/>

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=700&size=22&duration=2200&pause=100000&repeat=false&color=39FF14&center=false&vCenter=true&width=420&height=32&lines=PHASE_01+%3A%3A+RECON" alt="Phase 01"/>

I enjoy building AI systems from end to end—developing and evaluating models, designing the backend that powers them, building intuitive frontends, and deploying applications that solve real problems. My interests span LLMs, retrieval-augmented generation, AI security, and full-stack engineering, but I'm just as interested in the infrastructure and developer tooling that make AI systems reliable and practical.

Whether it's exploring new ideas through research or shipping production-ready projects, I enjoy turning complex problems into software that's useful, secure, and built to last.


<br/>

<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/>

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=700&size=22&duration=2200&pause=100000&repeat=false&color=00E5FF&center=false&vCenter=true&width=380&height=32&lines=PHASE_02+%3A%3A+STACK_TRACE" alt="Phase 02"/>

**Languages**

<img src="https://skillicons.dev/icons?i=python,js,r&theme=dark" />

**ML / Research**

<img src="https://skillicons.dev/icons?i=pytorch,sklearn,huggingface&theme=dark" />

**Backend & Frontend**

<img src="https://skillicons.dev/icons?i=fastapi,flask,react&theme=dark" />

**Databases**

<img src="https://skillicons.dev/icons?i=mysql,postgres&theme=dark" />

**DevOps & Tooling**

<img src="https://skillicons.dev/icons?i=git,docker,githubactions,vscode&theme=dark" />

<br/>

<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/>

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=700&size=22&duration=2200&pause=100000&repeat=false&color=FF9D00&center=false&vCenter=true&width=420&height=32&lines=PHASE_03+%3A%3A+SYSTEMS_SHIPPED" alt="Phase 03"/>

<table>

<tr>
<td width="270" valign="top">
<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/pin-cross-phase-defense-framework.svg" width="250"/>
</td>
<td valign="top">

### [cross-phase-defense-framework](https://github.com/aleenagibi/cross-phase-defense-framework)
![DistilBERT](https://img.shields.io/badge/-DistilBERT-0D1117?style=flat-square) ![GPT2](https://img.shields.io/badge/-GPT--2-0D1117?style=flat-square) ![FGSM](https://img.shields.io/badge/-FGSM-0D1117?style=flat-square) ![PGD](https://img.shields.io/badge/-PGD-0D1117?style=flat-square) ![DeepFool](https://img.shields.io/badge/-DeepFool-0D1117?style=flat-square)

🏆 A defense framework built on the assumption that any *single* line of defense against LLM attacks will eventually fail — so it doesn't rely on one.

<details>
<summary><b>Read the full breakdown</b></summary><br/>

Most defenses against adversarial LLM attacks target one point in the pipeline — clean the training data, or harden the model, or filter the output — and attackers adapt around whichever single barrier is in front of them. This framework instead layers defense across three independent stages: **data sanitization** at ingestion (catching poisoned samples before they ever reach training), **adversarial training** during model development (exposing the model to perturbed inputs so it generalizes past them), and **runtime backdoor detection** at inference (flagging trigger-pattern inputs even if they slipped past the first two layers). An attacker now has to defeat three separate mechanisms instead of one.

Validated with a proof-of-concept on DistilBERT and GPT-2, simulating data-poisoning and backdoor attacks and benchmarking robustness against FGSM, PGD, and DeepFool adversarial methods on IMDB and AG News. The result won **Best Paper at ICEIBT Conference 2026** and is currently under review for WoS publication. As LLMs get embedded deeper into production systems, single-point defenses that only catch known attack signatures are a shrinking target — the bet here is that resilience has to come from the architecture of the defense, not any one perfect filter.

</details>
</td>
</tr>

<tr><td colspan="2"><img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/></td></tr>

<tr>
<td width="270" valign="top">
<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/pin-hybrid-ai-chatbot.svg" width="250"/>
</td>
<td valign="top">

### [hybrid-ai-chatbot](https://github.com/aleenagibi/hybrid-ai-chatbot)
![Python](https://img.shields.io/badge/-Python-0D1117?style=flat-square&logo=python&logoColor=39FF14) ![RAG](https://img.shields.io/badge/-RAG-0D1117?style=flat-square) ![LLM](https://img.shields.io/badge/-LLM-0D1117?style=flat-square) ![Embeddings](https://img.shields.io/badge/-Embeddings-0D1117?style=flat-square)

A chatbot that knows when it doesn't know — and routes instead of guessing.

<details>
<summary><b>Read the full breakdown</b></summary><br/>

Plain LLM chatbots hallucinate confidently, and bolting on retrieval doesn't fully fix that — if the system always answers from whatever got retrieved, irrelevant context gets treated as gospel just as often as good context does. This project puts a routing layer in front of generation: per query, it decides whether to answer from retrieved context, call an external API for something that needs to be current or exact, or escalate to a specialized module rather than force a generic LLM answer.

That routing decision is the actual engineering problem — it's effectively a lightweight orchestrator sitting in front of the model rather than treating the LLM as the whole system. The architecture is also naturally extensible: new tools or data sources can be added at the routing layer without retraining or fine-tuning anything, which is closer to how production LLM systems are actually built than a single-shot RAG demo.

</details>
</td>
</tr>

<tr><td colspan="2"><img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/></td></tr>

<tr>
<td width="270" valign="top">
<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/pin-honeytrap.svg" width="250"/>
</td>
<td valign="top">

### [HoneyTrap](https://github.com/aleenagibi/HoneyTrap)
![Python](https://img.shields.io/badge/-Python-0D1117?style=flat-square&logo=python&logoColor=39FF14) ![sklearn](https://img.shields.io/badge/-scikit--learn-0D1117?style=flat-square&logo=scikitlearn&logoColor=39FF14) ![AWS](https://img.shields.io/badge/-AWS-0D1117?style=flat-square&logo=amazonaws&logoColor=39FF14) ![RandomForest](https://img.shields.io/badge/-Random%20Forest-0D1117?style=flat-square)

Feeding a honeypot's raw noise to a classifier instead of a human analyst.

<details>
<summary><b>Read the full breakdown</b></summary><br/>

Honeypots generate huge volumes of attack telemetry, and most of it is noise — the hard part isn't collecting the data, it's turning raw network/host event logs into features a model can actually learn from. This project engineers those features from AWS honeypot data and trains a Random Forest classifier to separate benign activity from malicious traffic, reaching over **91% accuracy**.

The practical value is triage: a pipeline like this is what would sit in front of a security operations workflow, automatically surfacing the honeypot hits worth a human's attention instead of requiring someone to review every single one manually. It's the ML-modeling half of security work — evaluation methodology and feature engineering — kept deliberately separate from the cross-phase-defense-framework research, which is about LLM-specific attack surfaces rather than network intrusion detection.

</details>
</td>
</tr>

<tr><td colspan="2"><img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/></td></tr>

<tr>
<td width="270" valign="top">
<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/pin-fileguard.svg" width="250"/>
</td>
<td valign="top">

### [FileGuard](https://github.com/aleenagibi/FileGuard)
![JavaScript](https://img.shields.io/badge/-JavaScript-0D1117?style=flat-square&logo=javascript&logoColor=39FF14) ![Chrome](https://img.shields.io/badge/-Chrome%20Ext.-0D1117?style=flat-square&logo=googlechrome&logoColor=39FF14) ![ManifestV3](https://img.shields.io/badge/-Manifest%20V3-0D1117?style=flat-square) ![VirusTotal](https://img.shields.io/badge/-VirusTotal-0D1117?style=flat-square)

Malware scanning that happens before you click download, not after you're already infected.

<details>
<summary><b>Read the full breakdown</b></summary><br/>

Most malware scanning happens after a file is already sitting on disk. FileGuard intercepts earlier — it injects inline "Scan" buttons directly into the Gmail UI via DOM observation (`MutationObserver`), so the check happens before the attachment ever touches your machine, and queries VirusTotal's multi-engine analysis for a verdict.

The engineering constraints are what make it more than a wrapper around one API call: attachments are hashed client-side (SHA-256) rather than uploaded anywhere, so the file itself never leaves your machine — only its hash does, which matters for privacy and for staying inside VirusTotal's free-tier upload limits on large files. A rate-limiting queue keeps the extension inside VirusTotal's request quotas, a batch "Scan All Attachments" mode handles multi-attachment emails with per-file progress and a summary report, and a settings panel lets users manage their own API key via the Chrome Storage API rather than hardcoding one.

</details>
</td>
</tr>

<tr><td colspan="2"><img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/></td></tr>

<tr>
<td width="270" valign="top">
<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/pin-blockchain-voting.svg" width="250"/>
</td>
<td valign="top">

### [Blockchain-Based-Voting-System](https://github.com/aleenagibi/Blockchain-Based-Voting-System)
![Python](https://img.shields.io/badge/-Python-0D1117?style=flat-square&logo=python&logoColor=39FF14) ![Flask](https://img.shields.io/badge/-Flask-0D1117?style=flat-square&logo=flask&logoColor=39FF14) ![SQLite](https://img.shields.io/badge/-SQLite-0D1117?style=flat-square&logo=sqlite&logoColor=39FF14) ![HMAC](https://img.shields.io/badge/-HMAC--SHA256-0D1117?style=flat-square) ![ChartJS](https://img.shields.io/badge/-Chart.js-0D1117?style=flat-square&logo=chartdotjs&logoColor=39FF14)

A voting system where the ledger proves the count without ever knowing who voted for what.

<details>
<summary><b>Read the full breakdown</b></summary><br/>

Electronic voting has two goals that are normally in tension: **auditability** (anyone should be able to verify the tally is honest) and **anonymity** (no one should be able to link a person to their vote). This project satisfies both at once rather than picking one. Auditability comes from a Proof-of-Authority chain where a block is only accepted once a configurable quorum (default 5 of 7) of HMAC-SHA256-signed validators agrees — no single party, including the system operator, can unilaterally rewrite the ledger. Anonymity comes from a coin-based model: each registered voter receives one spendable "voting coin" at registration, and only an anonymous token — never the voter's identity — is what actually gets written to the chain when that coin is spent.

That coin model also enforces one-vote-per-person at the *data layer*, not just the UI layer — meaning even if someone found a way around the frontend's session checks, the underlying ledger structure would still refuse a second vote from an already-spent coin. An admin/validator dashboard shows live tallies computed directly from the blockchain (not a separate database, avoiding any drift between "what's displayed" and "what's actually on the chain") plus full chain-integrity verification.

</details>
</td>
</tr>

<tr><td colspan="2"><img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/></td></tr>

<tr>
<td width="270" valign="top">
<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/pin-school-template-engine.svg" width="250"/>
</td>
<td valign="top">

### [school-template-engine](https://github.com/aleenagibi/school-template-engine)
![FastAPI](https://img.shields.io/badge/-FastAPI-0D1117?style=flat-square&logo=fastapi&logoColor=39FF14) ![React](https://img.shields.io/badge/-React-0D1117?style=flat-square&logo=react&logoColor=39FF14) ![FAISS](https://img.shields.io/badge/-FAISS-0D1117?style=flat-square) ![SentenceTransformers](https://img.shields.io/badge/-Sentence--Transformers-0D1117?style=flat-square) ![Babel](https://img.shields.io/badge/-Babel-0D1117?style=flat-square&logo=babel&logoColor=39FF14) ![Docker](https://img.shields.io/badge/-Docker-0D1117?style=flat-square&logo=docker&logoColor=39FF14)

Turns "copy-paste this section from another school's site" into a searchable, mergeable operation.

<details>
<summary><b>Read the full breakdown</b></summary><br/>

Grew directly out of a pattern I kept hitting during my Entab internship, building near-identical school websites over and over: the components you need almost always already exist somewhere in an old codebase, but finding them means either remembering exact file names or grepping through dozens of unfamiliar repos. This tool indexes reusable UI sections across a whole library of React codebases and makes them searchable by **what a component does**, not what it's named — a semantic search layer built on Sentence-Transformer embeddings and FAISS, so "staff directory grid with photos" finds the right component even if it was never labeled that.

The harder problem underneath is safe merging. Pulling components from different codebases risks CSS collisions and structurally invalid JSX if you naively concatenate files, so this uses automatic CSS selector scoping and a client-side, AST-based JSX merger built on Babel to combine components into one valid file — deliberately avoiding regex-based string manipulation, which breaks in ways that are hard to predict. I also evaluated using an LLM to do the merging and decided against it: an AST-based parser gives deterministic, structurally guaranteed correctness that a generative model can't promise, which matters when the output is going straight into a production website.

</details>
</td>
</tr>

<tr><td colspan="2"><img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/></td></tr>

<tr>
<td width="270" valign="top">
<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/pin-campus-path-finder.svg" width="250"/>
</td>
<td valign="top">

### [Campus_Path_Finder](https://github.com/aleenagibi/Campus_Path_Finder)
![Python](https://img.shields.io/badge/-Python-0D1117?style=flat-square&logo=python&logoColor=39FF14) ![Jupyter](https://img.shields.io/badge/-Jupyter-0D1117?style=flat-square&logo=jupyter&logoColor=39FF14) ![Graph](https://img.shields.io/badge/-Graph%20Algorithms-0D1117?style=flat-square)

Pathfinding you can actually watch happen, not just a printed shortest-path number.

<details>
<summary><b>Read the full breakdown</b></summary><br/>

Most people first learn BFS, DFS, and Dijkstra's algorithm from static diagrams and a final answer — this notebook game instead lets you place obstacles and weight edges on a campus-style graph and watch each algorithm's frontier expand step by step. That makes the trade-offs concrete instead of theoretical: BFS explores level-by-level regardless of cost, Dijkstra's accounts for edge weight and finds the true shortest path, and DFS can commit to a path early and miss the optimal one entirely — differences that are easy to state and hard to *feel* until you watch them happen side by side on the same graph.

</details>
</td>
</tr>

</table>

<sub>Also solving problems on [leetcode-solutions](https://github.com/aleenagibi/leetcode-solutions) between everything else.</sub>

<br/>

<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/>

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=700&size=22&duration=2200&pause=100000&repeat=false&color=FFD500&center=false&vCenter=true&width=460&height=32&lines=PHASE_04+%3A%3A+VERIFIED_RESEARCH" alt="Phase 04"/>

**Cross-Phase Defense Framework for Adversarial Attacks on Large Language Models**
🏆 Best Paper Award — ICEIBT Conference 2026 · Under review for WoS publication

A multi-layered defense strategy hardening LLMs at multiple stages of the pipeline — data sanitization, adversarial training, and backdoor detection — tested against simulated data-poisoning and backdoor attacks on DistilBERT using IMDB and AG News.

<br/>

<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/>

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=700&size=22&duration=2200&pause=100000&repeat=false&color=B388FF&center=false&vCenter=true&width=420&height=32&lines=PHASE_05+%3A%3A+IN_PROGRESS" alt="Phase 05"/>

**GreenLens** *(ongoing — final-year major project, now doubling as the basis for a second research paper)*. An agentic, carbon-aware LLM inference orchestrator: it embeds a task, predicts complexity/capability/carbon cost per candidate model, routes to the smallest model on the lowest-carbon deployment that meets the constraints, and explains the decision. Built on FAISS + Sentence-Transformers for task embedding, self-hosted inference via Ollama/vLLM, and live grid-carbon data.

<br/>

<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/>

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=700&size=22&duration=2200&pause=100000&repeat=false&color=39FF14&center=false&vCenter=true&width=460&height=32&lines=PHASE_06+%3A%3A+LIVE_MONITORING" alt="Phase 06"/>

<div align="center">

<!-- <img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/stats.svg" width="48%"/>
<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/top-langs.svg" width="30%"/>

<img src="https://streak-stats.demolab.com/?user=aleenagibi&hide_border=true&background=0D1117&ring=39FF14&fire=39FF14&currStreakLabel=39FF14&sideLabels=C9D1D9&currStreakNum=E6F7EC&sideNums=E6F7EC&dates=8B949E" width="80%"/> 

<br/><br/>-->

<!-- Snake animation — activate after enabling the workflow in .github/workflows/snake.yml (see SETUP.md) -->
<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/output/snake-dark.svg" width="100%"/>

</div>

<br/>

<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/>

<div align="center"><br/>

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=500&size=14&duration=2000&pause=1500&color=6E7681&center=true&vCenter=true&repeat=true&width=560&lines=%3E+connection+closed+%2F%2F+thanks+for+scanning;reach+me+%E2%80%94" alt="footer"/>

<br/>

[![Gmail](https://img.shields.io/badge/-aleenagibi2005%40gmail.com-0D1117?style=flat-square&logo=gmail&logoColor=39FF14)](mailto:aleenagibi2005@gmail.com)
[![LinkedIn](https://img.shields.io/badge/-linkedin%2Fin%2Faleenagibi2005-0D1117?style=flat-square&logo=linkedin&logoColor=39FF14)](https://www.linkedin.com/in/aleenagibi2005/)

</div>
