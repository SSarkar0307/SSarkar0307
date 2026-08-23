<!--
═══════════════════════════════════════════════════════════════════════════════
  SOHAN SARKAR — github.com/SSarkar0307
  Six values still need filling. Search for  «FILL»  — that's all of them.
  Setup order + what breaks: SETUP.md
  Palette — ink #0D1117 · marigold #F0A202 · ember #D64933 · slate #8B949E
═══════════════════════════════════════════════════════════════════════════════
-->

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="./assets/header.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/header-light.svg">
  <img alt="Sohan Sarkar — backend and distributed systems engineer" src="./assets/header.svg" width="100%">
</picture>

<br>

<img alt="Backend and distributed systems engineer. Currently building an event-driven collaboration platform." src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&pause=1500&color=F0A202&center=true&vCenter=true&width=780&height=42&lines=Node.js+%C2%B7+Kafka+%C2%B7+Redis+%C2%B7+Postgres+%C2%B7+AWS;LeetCode+Knight+%E2%80%94+1880%2B%2C+800%2B+problems+solved;Built+AI+governance+pipelines+%E2%80%94+approvals%2C+policy%2C+audit;Building%3A+an+event-driven+workspace+for+engineering+teams">

<br>

<a href="https://www.linkedin.com/in/sohan-sarkar-2726b5327/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-Connect-8B949E?style=flat-square&labelColor=0D1117&logo=linkedin&logoColor=8B949E"></a>
<a href="https://leetcode.com/u/lackblack99/"><img alt="LeetCode" src="https://img.shields.io/badge/LeetCode-Knight%201880%2B-F0A202?style=flat-square&labelColor=0D1117&logo=leetcode&logoColor=F0A202"></a>
<a href="mailto:sarkarsohan.3706@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-sarkarsohan.3706-8B949E?style=flat-square&labelColor=0D1117&logo=gmail&logoColor=8B949E"></a>

</div>

<br>

## ▌ Who

I build backends — specifically the parts that have to stay correct once things go concurrent.
Event-driven services, message queues, caches, and the design work underneath them: where state
lives, what the interfaces promise, and what happens when a node comes back after being gone for
ten minutes.

Three things have most of my attention right now.

**Distributed systems.** I'm building a collaboration platform on CRDTs and a Kafka event bus,
where the interesting work is the reconnect path and the conflict resolution, not the happy path.

**System design, especially low-level.** I work through LLD problems in the open and write down the
reasoning — why this abstraction, what breaks at scale — rather than just committing the class
diagram. It's the part of engineering I find genuinely fun.

**Infrastructure.** Publish-and-distribute pipelines, storage layers, versioning, the plumbing that
everything else assumes works.

Most recently I was a **backend developer intern at [OpsAI](https://www.linkedin.com/company/opsai)**,
building the APIs and governance pipelines between AI agents and enterprise systems — role-based
approvals, policy checks, risk classification, audit trails. Compliance code is unglamorous and
completely unforgiving, which turned out to be good training.

Competitive programming is where the instinct came from. 1000+ problems solved, LeetCode Knight at
1880+. It taught me to go looking for the input that breaks something before I go looking for the
one that works — which is most of what backend engineering turns out to be.

Studying **Electrical & Computer Engineering at Jamia Millia Islamia** and **BS Data Science at
IIT Madras**, concurrently, since 2024.

**→ Fastest way to reach me: [sarkarsohan.3706@gmail.com](mailto:sarkarsohan.3706@gmail.com)**

<br>

## ▌ Now

<sub>Last reviewed <b>August 2026</b>.</sub>

| | |
|:--|:--|
| **Building** | «GOTHAM» — an event-driven workspace for engineering teams. CRDT collaborative editing, Kafka event bus, OpenSearch, and a knowledge graph that links docs to the PRs, incidents and ADRs behind them. Public in 1–2 months. |
| **Recently shipped** | AI-execution governance at OpsAI — policy engine, risk classification, audit logging |
| **Practising daily** | Low-level design problems → [`Low-Level-Design`](https://github.com/SSarkar0307/Low-Level-Design) |
| **Learning** | Distributed consensus and CRDTs, properly rather than by vibes |
| **Open to** | Backend / distributed-systems roles — available now |

<br>

## ▌ Ship log

<div align="center">

<a href="https://github.com/SSarkar0307/npm-package-upload-infra">
  <img width="49%" alt="npm-package-upload-infra"
       src="https://github-stats-extended.vercel.app/api/pin/?username=SSarkar0307&repo=npm-package-upload-infra&bg_color=00000000&title_color=F0A202&text_color=8B949E&icon_color=D64933&hide_border=true&border_radius=6">
</a>
<a href="https://github.com/SSarkar0307/Low-Level-Design">
  <img width="49%" alt="Low-Level-Design"
       src="https://github-stats-extended.vercel.app/api/pin/?username=SSarkar0307&repo=Low-Level-Design&bg_color=00000000&title_color=F0A202&text_color=8B949E&icon_color=D64933&hide_border=true&border_radius=6">
</a>

<!-- «FILL» Add two more pins here if NavVision / the YouTube classifier have public repos.
     Copy a block above and change &repo=<name> and the href. If they don't exist as
     public repos, leave this at two — two real cards beat four broken ones. -->

</div>

<br>

**`npm-package-upload-infra`** — Publish-and-distribute infrastructure for npm packages: the upload
path, versioning, and the storage layer behind it. <sub>`Node.js` · `AWS`</sub>

**`Low-Level-Design`** — Working through LLD interview problems in the open — parking lot, rate
limiter, elevator, and the rest — with the design reasoning written down, not just the code.
Updated most weeks. <sub>`Java/C++` · `design patterns`</sub>

<br>

### In progress — «GOTHAM»

An event-driven collaboration workspace built for engineering teams specifically, not a Notion clone.
The thesis is that **everything should be connected**: a document knows about the pull requests,
incidents, ADRs and people attached to it, so you can ask *why* an architectural decision was made
and trace the answer.

| | |
|:--|:--|
| **Real-time** | CRDT-based collaborative editing — concurrent writes, conflict resolution, offline edits, presence, version history |
| **Event bus** | Kafka. Page edits, uploads, comments and tasks emit events; notification, search, analytics and audit services consume independently |
| **State** | Redis for sessions, caching, rate limiting, distributed locks and Pub/Sub presence |
| **Search** | OpenSearch, populated asynchronously off the event stream |
| **Storage** | S3 + CloudFront |
| **AI** | A subsystem, not the pitch — semantic search, summaries, "ask this workspace" |

Deliberately built in slices rather than all at once. Repo goes public when the collaborative
editing layer survives a reconnect storm.

<br>

## ▌ Competitive

<div align="center">

<img width="58%" alt="LeetCode statistics"
     src="https://leetcard.jacoblin.cool/lackblack99?theme=light,dark&font=JetBrains%20Mono&ext=heatmap">

</div>

| | |
|:--|:--|
| 🥇 | **1st** — Paradox ML Challenge (Freshers) |
| 🥇 | **1st of 200** — ACPC 2K25, ICPC-style contest, ABES College of Engineering |
| 🥇 | **Winner** — Debug Arena 2026, DSA contest, ARSDC Delhi University |
| 🥈 | **2nd runner-up** — Synapse-AI'26, AI×Sports hackathon at DTU, 350+ participants |
| 🎖 | **Finalist** — HackJMI 2025 (NavVision, CV navigation aid for the visually impaired) |
| 🎖 | **Runner-up** — Algo Clash 3X, GDG JMI |
| 🎖 | **Finalist** in Several Other Hackathons & Contests...|

<br>

## ▌ Telemetry

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="https://github-stats-extended.vercel.app/api?username=SSarkar0307&show_icons=true&include_all_commits=true&rank_icon=percentile&hide_border=true&bg_color=00000000&title_color=F0A202&text_color=C9D1D9&icon_color=D64933&ring_color=F0A202&custom_title=Contribution%20readout">
  <source media="(prefers-color-scheme: light)" srcset="https://github-stats-extended.vercel.app/api?username=SSarkar0307&show_icons=true&include_all_commits=true&rank_icon=percentile&hide_border=true&bg_color=00000000&title_color=B87400&text_color=57606A&icon_color=B0341F&ring_color=B87400&custom_title=Contribution%20readout">
  <img height="196" alt="GitHub statistics" src="https://github-stats-extended.vercel.app/api?username=SSarkar0307&show_icons=true&include_all_commits=true&rank_icon=percentile&hide_border=true&bg_color=00000000&title_color=F0A202&text_color=C9D1D9&icon_color=D64933&ring_color=F0A202">
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="https://github-stats-extended.vercel.app/api/top-langs/?username=SSarkar0307&layout=donut&langs_count=6&size_weight=0.5&count_weight=0.5&hide_border=true&bg_color=00000000&title_color=F0A202&text_color=C9D1D9&custom_title=Where%20the%20bytes%20go">
  <source media="(prefers-color-scheme: light)" srcset="https://github-stats-extended.vercel.app/api/top-langs/?username=SSarkar0307&layout=donut&langs_count=6&size_weight=0.5&count_weight=0.5&hide_border=true&bg_color=00000000&title_color=B87400&text_color=57606A&custom_title=Where%20the%20bytes%20go">
  <img height="196" alt="Most used languages" src="https://github-stats-extended.vercel.app/api/top-langs/?username=SSarkar0307&layout=donut&langs_count=6&hide_border=true&bg_color=00000000&title_color=F0A202&text_color=C9D1D9">
</picture>

<!--
  ┌─ BULLETPROOF MODE ──────────────────────────────────────────────────────┐
  │ The two cards above hit a public API that can rate-limit. The `cards`   │
  │ job in .github/workflows/profile.yml generates the same SVGs INTO this  │
  │ repo, where GitHub serves them itself and they can never 429.           │
  │ Once that job has run, delete the two picture blocks and uncomment:   │
  └─────────────────────────────────────────────────────────────────────────┘
<img height="196" alt="GitHub statistics"   src="./assets/stats.svg">
<img height="196" alt="Most used languages" src="./assets/top-langs.svg">
-->

<br><br>

<img width="76%" alt="Contribution streak"
     src="https://streak-stats.demolab.com?user=SSarkar0307&hide_border=true&background=00000000&stroke=30363D&ring=F0A202&fire=D64933&currStreakNum=F0A202&sideNums=8B949E&currStreakLabel=F0A202&sideLabels=8B949E&dates=8B949E&date_format=j%20M%5B%20Y%5D">

<br><br>

<img width="98%" alt="Contribution activity graph for the last 31 days"
     src="https://github-readme-activity-graph.vercel.app/graph?username=SSarkar0307&bg_color=00000000&color=8B949E&line=F0A202&point=D64933&area=true&area_color=F0A202&hide_border=true&custom_title=Commits%20per%20day">

</div>

<details>
<summary><b>▌ More telemetry</b> — the year as a city, the year as lunch, per-language breakdowns</summary>

<br>

<div align="center">

<img width="98%" alt="Isometric 3D contribution calendar" src="./profile-3d-contrib/profile-night-rainbow.svg">

<br><br>

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="https://raw.githubusercontent.com/SSarkar0307/SSarkar0307/output/snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/SSarkar0307/SSarkar0307/output/snake.svg">
  <img width="98%" alt="A snake eating my contribution graph"
       src="https://raw.githubusercontent.com/SSarkar0307/SSarkar0307/output/snake.svg">
</picture>

<br><br>

<img width="49%" alt="Repositories per language"
     src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=SSarkar0307&theme=github_dark">
<img width="49%" alt="Most committed language"
     src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=SSarkar0307&theme=github_dark">
<img width="49%" alt="Profile statistics summary"
     src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=SSarkar0307&theme=github_dark">
<img width="49%" alt="Most productive time of day"
     src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=SSarkar0307&theme=github_dark&utcOffset=5.5">

<br><br>

<img width="90%" alt="Full metrics infographic — calendar, languages, activity, habits"
     src="./assets/metrics.svg">

</div>

</details>

<br>

## ▌ Stack

<sub>Ordered by what I'd reach for first, not alphabetically.</sub>

<table>
<tr>
<td width="160"><b>Backend</b></td>
<td>
<img alt="Node.js, Express, Python, FastAPI, Flask" src="https://skillicons.dev/icons?i=nodejs,express,py,fastapi,flask&theme=dark">
<br><sub>Also <b>Fastify</b> · REST API design · async processing</sub>
</td>
</tr>
<tr>
<td><b>Distributed &amp; data</b></td>
<td>
<img alt="Kafka, Redis, PostgreSQL, MongoDB" src="https://skillicons.dev/icons?i=kafka,redis,postgres,mongodb&theme=dark">
<br><sub>Also <b>OpenSearch</b> · CRDTs · event-driven architecture · distributed locks</sub>
</td>
</tr>
<tr>
<td><b>Cloud &amp; infra</b></td>
<td>
<img alt="AWS, Docker, Linux, Git, GitHub Actions" src="https://skillicons.dev/icons?i=aws,docker,linux,git,githubactions&theme=dark">
<br><sub>S3 · CloudFront · CI/CD</sub>
</td>
</tr>
<tr>
<td><b>Languages</b></td>
<td>
<img alt="C++, Java, Python, JavaScript, TypeScript" src="https://skillicons.dev/icons?i=cpp,java,py,js,ts&theme=dark">
<br><sub>C++ / Python for contests, Java for LLD, JS/TS for everything else</sub>
</td>
</tr>
<tr>
<td><b>Design</b></td>
<td>
<sub>Low-level design · design patterns · system design · API contracts</sub>
</td>
</tr>
<tr>
<td><b>Frontend</b><br><sub>secondary</sub></td>
<td>
<img alt="React, Next.js, Tailwind, Three.js" src="https://skillicons.dev/icons?i=react,nextjs,tailwind,threejs&theme=dark">
<br><sub>GSAP · WebGL shaders · Locomotive Scroll — motion-heavy client work</sub>
</td>
</tr>
<tr>
<td><b>ML</b><br><sub>coursework</sub></td>
<td>
<img alt="scikit-learn, OpenCV, PyTorch" src="https://skillicons.dev/icons?i=sklearn,opencv,pytorch&theme=dark">
<br><sub>LSTM classification · YOLO object detection</sub>
</td>
</tr>
</table>

<br>

<details>
<summary><b>▌ Recent activity</b></summary>

<br>

<!--START_SECTION:activity-->
<!-- Auto-filled by the `activity` job on first run. -->
<!--END_SECTION:activity-->

</details>

<br>

## ▌ Working together

I'm looking for backend and distributed-systems work and I'm available now. If you're building
something where correctness under concurrency actually matters — event pipelines, real-time state,
anything with a hard consistency story — I'd like to hear about it.

<div align="center">
<br>
<a href="mailto:sarkarsohan.3706@gmail.com">
  <img alt="Email me" src="https://img.shields.io/badge/→%20%20sarkarsohan.3706@gmail.com%20%20←-F0A202?style=for-the-badge&labelColor=0D1117">
</a>
<br><br>
<sub><i>"The bug is in the case you didn't write a test for."</i></sub>
</div>

<img width="100%" alt=""
     src="https://capsule-render.vercel.app/api?type=waving&section=footer&height=120&color=0:0D1117,55:1A1F2B,100:F0A202">