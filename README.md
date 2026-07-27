<div align="center">

<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/glitch-hero.svg" width="100%" alt="Aleena Gibi — animated hero"/>

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=500&size=15&duration=2600&pause=700&color=8B949E&center=true&vCenter=true&repeat=true&width=760&lines=%24+whoami;final-year+B.Sc.+(Hons.+Research)+Data+Science+%26+AI+%40+CHRIST+Delhi+NCR;%24+tail+-f+currently.log;building+GreenLens+%E2%80%94+a+carbon-aware+LLM+inference+router" alt="typing terminal"/>

</div>

<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/>

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=700&size=22&duration=2200&pause=100000&repeat=false&color=39FF14&center=false&vCenter=true&width=420&height=32&lines=PHASE_01+%3A%3A+RECON" alt="Phase 01"/>

Final-year AI/ML undergraduate who builds across the whole stack instead of staying in one lane — training and evaluating models, shipping the backend and frontend around them, and occasionally hardening the whole thing against the ways it can fail. That range shows up in what I build: a Best Paper–winning defense framework for adversarial attacks on LLMs, a RAG-based chatbot, a carbon-aware inference router, and a couple of systems projects that have nothing to do with ML at all. Currently aiming for a master's in applied AI/ML/NLP in Germany.

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

**DevOps & Tooling**

<img src="https://skillicons.dev/icons?i=git,docker,githubactions,vscode,figma&theme=dark" />

<br/>

<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/scanline.svg" width="100%"/>

<br/>

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=700&size=22&duration=2200&pause=100000&repeat=false&color=FF9D00&center=false&vCenter=true&width=420&height=32&lines=PHASE_03+%3A%3A+SYSTEMS_SHIPPED" alt="Phase 03"/>

### [cross-phase-defense-framework](https://github.com/aleenagibi/cross-phase-defense-framework)
🏆 **Best Paper, ICEIBT 2026** — the research repo behind my paper. A multi-layered defense against adversarial attacks on LLMs, hardening the pipeline at three separate stages — data sanitization, adversarial training, and runtime backdoor detection — instead of relying on any single defense. Benchmarked on DistilBERT/GPT-2 against FGSM, PGD, and DeepFool attacks on IMDB and AG News.

### [hybrid-ai-chatbot](https://github.com/aleenagibi/hybrid-ai-chatbot)
A retrieval-augmented chatbot that doesn't just generate — it decides. Routing logic picks per-query whether to answer from retrieved context, call an external API, or hand off to a specialized module, which keeps responses grounded instead of hallucinated.

### [HoneyTrap](https://github.com/aleenagibi/HoneyTrap)
Real-time attack detection trained on AWS honeypot telemetry. Feature-engineered a Random Forest classifier that separates benign from malicious traffic at 91%+ accuracy — the ML side of security work, versioned separately from the defense-framework research.

### [FileGuard](https://github.com/aleenagibi/FileGuard)
A Chrome extension (Manifest V3) that scans Gmail attachments against VirusTotal before you ever click download. Client-side SHA-256 hashing, a rate-limited queue to survive VirusTotal's free-tier API limits, and a batch "scan all attachments" mode with per-file progress.

### [Blockchain-Based-Voting-System](https://github.com/aleenagibi/Blockchain-Based-Voting-System)
A Proof-of-Authority voting platform where a block only gets accepted once a quorum of HMAC-signed validators agrees. Voter identity and cast ballots are deliberately kept apart — each registered voter gets a single spendable "voting coin," and only the anonymous token, never the voter ID, touches the chain.

### [school-template-engine](https://github.com/aleenagibi/school-template-engine)
Grew directly out of a repetitive pattern I kept hitting during my Entab internship: rebuilding near-identical sections across dozens of school websites. This full-stack tool (FastAPI + React) indexes reusable UI sections from a library of codebases and lets you semantically search and reassemble them into a new template — search by what a section *does*, not what it's named.

### [Campus_Path_Finder](https://github.com/aleenagibi/Campus_Path_Finder)
An interactive notebook game visualizing BFS, DFS, and Dijkstra's algorithm across a campus graph — built to make pathfinding trade-offs visible step by step rather than just correct.

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

<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/stats.svg" width="48%"/>
<img src="https://raw.githubusercontent.com/aleenagibi/aleenagibi/main/assets/top-langs.svg" width="30%"/>

<img src="https://streak-stats.demolab.com/?user=aleenagibi&hide_border=true&background=0D1117&ring=39FF14&fire=39FF14&currStreakLabel=39FF14&sideLabels=C9D1D9&currStreakNum=E6F7EC&sideNums=E6F7EC&dates=8B949E" width="80%"/>

<br/><br/>

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
