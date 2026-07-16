  <!-- ══════════════ MIDNIGHT ATELIER · design spec in DESIGN.md ══════════════ -->

<!-- ══════════════ 00 — HERO ARCHITECTURE ══════════════ -->
<div align="center">
  <img alt="typing pitch" src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=1000&color=A78BFA&center=true&vCenter=true&width=600&height=40&lines=FULL-STACK+ENGINEER;OBSESSED+WITH+SUB-50ms+SYSTEMS;BUILDING+OFF+THE+HOT+PATH;COMPETITIVE+PROGRAMMER"/>

  <br/><br/>

  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" height="28"/>
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" height="28"/>
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" height="28"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" height="28"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" height="28"/>

  <br/><br/>

  <a href="https://kartik-portfolio-6k36.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-black?style=for-the-badge&logo=react&logoColor=white" height="35"/></a>&nbsp;
  <a href="https://www.linkedin.com/in/kartik-bhargava-248796257"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" height="35"/></a>&nbsp;
  <a href="mailto:kartikbhargava1111@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" height="35"/></a>&nbsp;
  <a href="https://github.com/Consoder?tab=repositories"><img src="https://img.shields.io/badge/GitHub_Repos-181717?style=for-the-badge&logo=github&logoColor=white" height="35"/></a>

</div>

<!-- ══════════════ 01 — THE ENGINEER ══════════════ -->
<h2 align="left">
  <img src="https://img.shields.io/badge/01._THE_ENGINEER-121212?style=flat-square&fontName=Cinzel&size=34&fontColor=A78BFA&color=121212" alt="01. The Engineer" height="34" />
</h2>

<table width="100%">
<tr>
<td width="55%" valign="top">

```typescript
const kartik = {
  location: "Jaipur, IN — remote-ready",
  education: "B.Tech CSE '27 · SKIT · 8.3 CGPA",

  languages: ["C++", "Python", "JavaScript", "SQL", "C"],
  backend:   ["Node", "Express", "FastAPI"],
  frontend:  ["React", "Next.js", "Tailwind"],
  data:      ["PostgreSQL", "MongoDB", "Redis"],
  infra:     ["Docker", "AWS", "GitHub Actions"],

  dsa: { solved: 385, medium: 181, hard: 34 },

  obsession: "systems where the hot path never blocks",
  hireable: true,
};
```

</td>
<td width="45%" valign="middle" align="center">

<img src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif" width="100%" alt="coding"/>

</td>
</tr>
</table>

<br/>

<!-- ══════════════ 02 — ARCHITECTURE ══════════════ -->

<img src="assets/h-02.svg" width="100%" alt="02 — Architecture"/>

```mermaid
%%{init: {'theme':'dark','themeVariables':{'primaryColor':'#1a0533','primaryTextColor':'#e8d5ff','primaryBorderColor':'#8b5cf6','lineColor':'#a78bfa','fontFamily':'monospace','clusterBkg':'#0d001a'}}}%%
flowchart LR
    U(("👤 click")) --> API["Express API"]
    API --> C{"Redis<br/>cache hit?"}
    C -->|"yes · O(1)"| R[["⚡ 301 redirect<br/><b>sub-50ms</b>"]]
    C -->|miss| M[("MongoDB")] --> W["warm cache"] --> R
    API -.->|"fire & forget"| Q[/"BullMQ queue"/]
    subgraph BG ["⚙ off the hot path"]
        Q --> WK["worker"]
        WK --> GEO["geo-IP + UA<br/>fingerprint"]
        GEO --> AGG[("Mongo<br/>aggregations")]
        AGG --> DASH["📊 Recharts<br/>dashboard"]
    end
```

<div align="center"><sup>Every click enqueues a BullMQ job — workers do the heavy lifting off the hot path, so the redirect never waits for analytics. <a href="https://github.com/Consoder/Pulse.io"><b>→ read the code</b></a></sup></div>

<br/>

<!-- ══════════════ 03 — SELECTED WORK ══════════════ -->

<img src="assets/h-03.svg" width="100%" alt="03 — Selected Work"/>

<table width="100%">
<tr>
<td width="33%" valign="top">

<h3 align="center">⚡ Pulse.io</h3>
<p align="center"><sub><samp>LINK INTELLIGENCE ENGINE</samp></sub></p>

Sub-50ms redirects (architecture ↑). JWT + Google OAuth, MongoDB aggregation pipelines for geo / device / campaign breakdowns, Recharts + Framer Motion dashboard.

<p align="center"><code>React</code> <code>Node</code> <code>Express</code> <code>MongoDB</code> <code>Redis</code> <code>BullMQ</code></p>

<p align="center"><a href="https://github.com/Consoder/Pulse.io"><b>→ repository</b></a></p>

</td>
<td width="33%" valign="top">

<h3 align="center">🔍 Code Analysis Platform</h3>
<p align="center"><sub><samp>AI CODE REVIEW · 7 LANGUAGES</samp></sub></p>

Bug detection, Big-O analysis, quality scoring. Redis cache keyed on SHA-256 of source — repeat analysis drops from 2–8s to <b>~40ms</b>. JWT + OAuth, rate limiting, PostgreSQL.

<p align="center"><code>Next.js 14</code> <code>FastAPI</code> <code>Redis</code> <code>PostgreSQL</code></p>

<p align="center"><a href="https://github.com/Consoder/ROASTCODE"><b>→ repository</b></a></p>

</td>
<td width="33%" valign="top">

<h3 align="center">🚗 Vision Navigation</h3>
<p align="center"><sub><samp>BEHAVIORAL CLONING CNN</samp></sub></p>

NVIDIA-style end-to-end CNN, 4,500+ labeled frames → <b>121K params, 94.1% val accuracy</b>, real-time CPU inference. Pygame sim with Grad-CAM showing what the model watches while steering.

<p align="center"><code>Python</code> <code>TensorFlow</code> <code>OpenCV</code> <code>Pygame</code></p>

<p align="center"><a href="https://github.com/Consoder/Vision-Based-Autonomous-Navigation-System"><b>→ repository</b></a></p>

</td>
</tr>
</table>

<div align="center"><sub>ALSO — <a href="https://github.com/Consoder/saas-notes-app"><b>saas-notes-app</b></a> · multi-tenant API, JWT + RBAC &nbsp;/&nbsp; <a href="https://github.com/Consoder/SMS-IDENTIFIER"><b>SMS-IDENTIFIER</b></a> · TF-IDF spam classifier</sub></div>

<br/>

<!-- ══════════════ 04 — EXPERIENCE ══════════════ -->

<img src="assets/h-04.svg" width="100%" alt="04 — Experience"/>

<table width="100%">
<tr>
<td width="22%" align="center" valign="middle"><samp><b>MAY–JUN<br/>2026</b></samp></td>
<td width="78%" valign="middle">

<b>Software Engineer — Full-Stack Intern</b> · Wisflux Pvt. Ltd<br/>
<sub>Secure REST APIs, auth/authorization & backend features for a scalable MERN link-management platform · Agile/Scrum · code reviews · performance optimization</sub>

</td>
</tr>
<tr>
<td align="center" valign="middle"><samp><b>MAY–JUL<br/>2025</b></samp></td>
<td valign="middle">

<b>Python & Machine Learning Intern</b> · KisTechno Software Pvt. Ltd<br/>
<sub>End-to-end self-driving simulator — data collection, training, evaluation → 94%+ accuracy · Grad-CAM explainability added on mentor feedback</sub>

</td>
</tr>
</table>

<table width="100%">
<tr>
<td width="50%" align="center" valign="top">

<samp>HONOURS</samp>

🥈 IEEE Hackathon — <b>2nd Place</b><br/><sub>working prototype + go-to-market strategy</sub>

🎤 DevOps Workshop <b>Coordinator</b> — <sub>100+ students</sub>

</td>
<td width="50%" align="center" valign="top">

<samp>CREDENTIALS</samp>

☁️ AWS Cloud Practitioner Essentials<br/><sub>EC2 · S3 · VPC · IAM</sub>

✨ Google Vertex AI — Prompt Design · 📊 Deloitte Data Analytics

</td>
</tr>
</table>

<br/>

<!-- ══════════════ 05 — THE STACK ══════════════ -->

<img src="assets/h-05.svg" width="100%" alt="05 — The Stack"/>

<table width="100%">
<tr>
<td align="center" width="22%"><samp>LANGUAGES</samp></td>
<td align="center"><img src="https://skillicons.dev/icons?i=cpp,python,js,c,mysql&theme=dark"/></td>
</tr>
<tr>
<td align="center"><samp>FRONTEND ×<br/>BACKEND</samp></td>
<td align="center"><img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,express,fastapi,tailwind&theme=dark"/></td>
</tr>
<tr>
<td align="center"><samp>DATA</samp></td>
<td align="center"><img src="https://skillicons.dev/icons?i=postgres,mongodb,redis&theme=dark"/></td>
</tr>
<tr>
<td align="center"><samp>TOOLS × CLOUD</samp></td>
<td align="center"><img src="https://skillicons.dev/icons?i=git,github,githubactions,docker,aws,postman&theme=dark"/></td>
</tr>
</table>

<div align="center"><sub><samp>CORE CS — DSA · OOP · DBMS · OPERATING SYSTEMS · COMPUTER NETWORKS · REST · CI/CD</samp></sub></div>

<br/>

<!-- ══════════════ 06 — TELEMETRY ══════════════ -->

<img src="assets/h-06.svg" width="100%" alt="06 — Telemetry"/>

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=Consoder&show_icons=true&hide_border=true&bg_color=0d001a&title_color=a78bfa&text_color=e8d5ff&icon_color=C9A876&ring_color=8b5cf6"/>&nbsp;<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Consoder&layout=compact&hide_border=true&bg_color=0d001a&title_color=a78bfa&text_color=e8d5ff&langs_count=8"/>

<br/><br/>

<!-- CONTRIBUTION SNAKE — powered by .github/workflows/snake.yml -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Consoder/Consoder/output/github-contribution-grid-snake-dark.svg"/>
  <img alt="contribution snake" src="https://raw.githubusercontent.com/Consoder/Consoder/output/github-contribution-grid-snake-dark.svg"/>
</picture>

</div>

<br/>

<!-- ══════════════ SIGN-OFF ══════════════ -->

<div align="center">

<img src="https://media.giphy.com/media/L1R1tvI9svkIWwpVYr/giphy.gif" width="280" alt="typing"/>

<br/><br/>

<img src="assets/signoff.svg" width="60%" alt="Let's build something real."/>

<br/>

<a href="https://kartik-portfolio-6k36.vercel.app/"><img src="assets/btn-portfolio.svg" height="42" alt="Portfolio"/></a>&nbsp;
<a href="https://www.linkedin.com/in/kartik-bhargava-248796257"><img src="assets/btn-linkedin.svg" height="42" alt="LinkedIn"/></a>&nbsp;
<a href="mailto:kartikbhargava1111@gmail.com"><img src="assets/btn-email.svg" height="42" alt="Email"/></a>

<br/><br/>

<img src="assets/footer.svg" width="100%" alt="build fast · ship clean · make it real"/>

</div>
