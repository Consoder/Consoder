<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&height=70&color=0:0a0a0f,50:4c1d95,100:0a0a0f&custom_height=70" width="100%"/>
</div>

<table width="100%">
<tr>
<td width="30%" align="center" valign="middle">

<img src="https://user-images.githubusercontent.com/74038190/212750999-42ff8a64-dad8-4772-9648-849968543991.gif" width="220" alt="Kartik Bhargava"/>

</td>
<td width="70%" align="center" valign="middle">

<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=700&size=40&duration=1&pause=99999&color=E8D5FF&center=true&vCenter=true&width=560&height=56&lines=Kartik+Bhargava" alt="Kartik Bhargava"/>

<img src="https://readme-typing-svg.demolab.com?font=Great+Vibes&weight=400&size=26&duration=1&pause=99999&color=C9A876&center=true&vCenter=true&width=560&height=42&lines=Building+products+people+love+to+use" alt="tagline"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=15&duration=3000&pause=1000&color=A78BFA&center=true&vCenter=true&width=560&height=28&lines=status%3A+open+to+sde+%2F+full-stack+%2F+backend;location%3A+jaipur%2C+india+-+remote-ready;focus%3A+systems+where+the+hot+path+never+blocks" alt="status"/>

<br/>

<img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,fastapi,redis,postgres&theme=dark" height="42"/>

<br/><br/>

<a href="https://kartik-portfolio-6k36.vercel.app/"><img src="https://img.shields.io/badge/PORTFOLIO-1a0533?style=flat-square&labelColor=1a0533&color=1a0533&logoColor=C9A876" height="30"/></a>&nbsp;
<a href="https://www.linkedin.com/in/kartik-bhargava-248796257"><img src="https://img.shields.io/badge/LINKEDIN-1a0533?style=flat-square&logo=linkedin&logoColor=a78bfa" height="30"/></a>&nbsp;
<a href="mailto:kartikbhargava1111@gmail.com"><img src="https://img.shields.io/badge/EMAIL-1a0533?style=flat-square&logo=gmail&logoColor=a78bfa" height="30"/></a>&nbsp;
<a href="https://github.com/Consoder?tab=repositories"><img src="https://img.shields.io/badge/REPOS-1a0533?style=flat-square&logo=github&logoColor=a78bfa" height="30"/></a>

</td>
</tr>
</table>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&height=70&color=0:0a0a0f,50:4c1d95,100:0a0a0f&custom_height=70&section=footer" width="100%"/>
</div>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&height=2&color=0:C9A876,50:8b5cf6,100:C9A876" width="100%"/>
</div>

<br/>

<!-- ══════════════ 01 — THE ENGINEER ══════════════ -->

<h2 align="left">
  <img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=26&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=420&height=42&lines=01.+THE+ENGINEER" alt="01. The Engineer"/>
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

<img src="https://user-images.githubusercontent.com/74038190/212750147-854a394f-fee9-4080-9770-78a4b7ece53f.gif" width="100%" alt="coding"/>

</td>
</tr>
</table>

<br/>

<!-- ══════════════ 02 — THE ARCHITECTURE ══════════════ -->

<h2 align="left">
  <img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=26&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=460&height=42&lines=02.+THE+ARCHITECTURE" alt="02. The Architecture"/>
</h2>

<p><samp>PULSE.IO — A REDIRECT THAT NEVER WAITS FOR ANALYTICS</samp></p>

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

<p><sup>Every click enqueues a BullMQ job — workers do the heavy lifting off the hot path, so the redirect never waits for analytics. <a href="https://github.com/Consoder/Pulse.io"><b>→ read the code</b></a></sup></p>

<br/>

<!-- ══════════════ 03 — SELECTED WORKS ══════════════ -->

<h2 align="left">
  <img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=26&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=460&height=42&lines=03.+SELECTED+WORKS" alt="03. Selected Works"/>
</h2>

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

<!-- ══════════════ 04 — THE EXPERIENCE ══════════════ -->

<h2 align="left">
  <img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=26&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=460&height=42&lines=04.+THE+EXPERIENCE" alt="04. The Experience"/>
</h2>

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

<h2 align="left">
  <img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=26&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=420&height=42&lines=05.+THE+STACK" alt="05. The Stack"/>
</h2>

<table width="100%">
<tr>
<td align="center" width="20%"><samp>LANGUAGES</samp></td>
<td align="center" width="80%">&nbsp;<br/><img src="https://skillicons.dev/icons?i=cpp,python,js,c,mysql&theme=dark&perline=8" height="52"/><br/>&nbsp;</td>
</tr>
<tr><td colspan="2"><br/></td></tr>
<tr>
<td align="center"><samp>FRONTEND<br/>×<br/>BACKEND</samp></td>
<td align="center" width="80%">&nbsp;<br/><img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,express,fastapi,tailwind&theme=dark&perline=8" height="52"/><br/>&nbsp;</td>
</tr>
<tr><td colspan="2"><br/></td></tr>
<tr>
<td align="center"><samp>DATA</samp></td>
<td align="center" width="80%">&nbsp;<br/><img src="https://skillicons.dev/icons?i=postgres,mongodb,redis&theme=dark&perline=8" height="52"/><br/>&nbsp;</td>
</tr>
<tr><td colspan="2"><br/></td></tr>
<tr>
<td align="center"><samp>TOOLS<br/>×<br/>CLOUD</samp></td>
<td align="center" width="80%">&nbsp;<br/><img src="https://skillicons.dev/icons?i=git,github,githubactions,docker,aws,postman&theme=dark&perline=8" height="52"/><br/>&nbsp;</td>
</tr>
</table>

<div align="center"><sub><samp>CORE CS — DSA · OOP · DBMS · OPERATING SYSTEMS · COMPUTER NETWORKS · REST · CI/CD</samp></sub></div>

<br/>

<!-- ══════════════ 06 — TELEMETRY ══════════════ -->

<h2 align="left">
  <img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=26&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=420&height=42&lines=06.+TELEMETRY" alt="06. Telemetry"/>
</h2>

<div align="center">

<img src="https://img.shields.io/badge/DSA_SOLVED-385+-1a0533?style=for-the-badge&labelColor=1a0533&color=1a0533&logoColor=C9A876"/>&nbsp;
<img src="https://img.shields.io/badge/MEDIUM-181-1a0533?style=for-the-badge&labelColor=1a0533&color=1a0533&logoColor=C9A876"/>&nbsp;
<img src="https://img.shields.io/badge/HARD-34-1a0533?style=for-the-badge&labelColor=1a0533&color=1a0533&logoColor=C9A876"/>&nbsp;
<img src="https://img.shields.io/github/followers/Consoder?style=for-the-badge&label=FOLLOWERS&labelColor=1a0533&color=1a0533"/>

<br/><br/>

<!-- CONTRIBUTION SNAKE — needs .github/workflows/snake.yml + one manual Action run.
     Skipping that setup? Delete this <picture> block, it will 404 otherwise. -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Consoder/Consoder/output/github-contribution-grid-snake-dark.svg"/>
  <img alt="contribution snake" src="https://raw.githubusercontent.com/Consoder/Consoder/output/github-contribution-grid-snake-dark.svg"/>
</picture>

</div>

<br/>

<!-- ══════════════ SIGN-OFF ══════════════ -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&height=2&color=0:C9A876,50:8b5cf6,100:C9A876" width="100%"/>

</div>

<br/>

<table width="100%">
<tr>
<td width="30%" align="center" valign="middle">

<img src="https://user-images.githubusercontent.com/74038190/212750999-42ff8a64-dad8-4772-9648-849968543991.gif" width="200" alt="Kartik Bhargava"/>

</td>
<td width="70%" align="center" valign="middle">

<img src="https://readme-typing-svg.demolab.com?font=Great+Vibes&weight=400&size=32&duration=1&pause=99999&color=C9A876&center=true&vCenter=true&width=560&height=52&lines=Let's+build+something+real" alt="Let's build something real"/>

<br/>

<a href="https://kartik-portfolio-6k36.vercel.app/"><img src="https://img.shields.io/badge/PORTFOLIO-1a0533?style=flat-square&labelColor=1a0533&color=1a0533&logoColor=C9A876" height="30"/></a>&nbsp;
<a href="https://www.linkedin.com/in/kartik-bhargava-248796257"><img src="https://img.shields.io/badge/LINKEDIN-1a0533?style=flat-square&logo=linkedin&logoColor=a78bfa" height="30"/></a>&nbsp;
<a href="mailto:kartikbhargava1111@gmail.com"><img src="https://img.shields.io/badge/EMAIL-1a0533?style=flat-square&logo=gmail&logoColor=a78bfa" height="30"/></a>

</td>
</tr>
</table>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=140&color=0:0d001a,50:4c1d95,100:0a0a0f&section=footer&text=BUILD%20FAST%20·%20SHIP%20CLEAN%20·%20MAKE%20IT%20REAL&fontSize=15&fontColor=C9A876&fontAlignY=78" width="100%"/>

</div>

</div>
