<!-- ════════════════════════════ BOOT SEQUENCE ════════════════════════════ -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&height=3&color=0:C9A876,50:8b5cf6,100:C9A876" width="100%"/>

<br/><br/>

<img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/Consoder&h=140&w=140&fit=cover&mask=circle" width="140" alt="Kartik Bhargava"/>

<br/><br/>

<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=600&size=40&duration=1&pause=99999&color=E8D5FF&center=true&vCenter=true&width=720&height=58&lines=Kartik+Bhargava" />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=400&size=14&duration=2800&pause=900&color=C9A876&center=true&vCenter=true&width=720&lines=%24+whoami+%E2%86%92+full-stack+engineer+%C2%B7+B.Tech+CSE+'27+%C2%B7+SKIT+Jaipur;%24+cat+stack.txt+%E2%86%92+React+%C2%B7+Next.js+%C2%B7+Node+%C2%B7+FastAPI+%C2%B7+Redis+%C2%B7+Postgres;%24+status+%E2%86%92+%F0%9F%9F%A2+open+to+SDE+%2F+full-stack+%2F+backend+roles" />

<br/>

<kbd><a href="https://kartik-portfolio-6k36.vercel.app/">&nbsp;⌘ PORTFOLIO&nbsp;</a></kbd>&nbsp;&nbsp;
<kbd><a href="https://www.linkedin.com/in/kartik-bhargava-248796257">&nbsp;⟡ LINKEDIN&nbsp;</a></kbd>&nbsp;&nbsp;
<kbd><a href="mailto:kartikbhargava1111@gmail.com">&nbsp;◈ EMAIL&nbsp;</a></kbd>&nbsp;&nbsp;
<kbd><a href="#architecture">&nbsp;⚙ SEE THE ARCHITECTURE ↓&nbsp;</a></kbd>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=rect&height=3&color=0:C9A876,50:8b5cf6,100:C9A876" width="100%"/>

</div>

<!-- ════════════════════════════ RUNTIME ════════════════════════════ -->

## <samp>~/kartik $ cat profile.ts</samp>

<img align="right" width="360" src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif" alt="coding gif"/>

```typescript
const kartik = {
  location: "Jaipur, IN — remote-ready",
  education: "B.Tech CSE '27 · SKIT Jaipur · 8.3 CGPA",

  languages: ["C++", "Python", "JavaScript", "SQL", "C"],
  backend:   ["Node", "Express", "FastAPI", "REST"],
  frontend:  ["React", "Next.js", "Tailwind"],
  data:      ["PostgreSQL", "MongoDB", "Redis"],
  infra:     ["Docker", "AWS", "GitHub Actions"],

  dsa: { solved: 385, medium: 181, hard: 34 },

  obsession: "systems where the hot path never blocks",
  currentlyShipping: "AI code analysis platform",
  hireable: true,
};
```

<br clear="right"/>

<div align="center"><samp>─────── ✦ ───────</samp></div>

<!-- ════════════════════════════ ARCHITECTURE ════════════════════════════ -->

<a id="architecture"></a>

## <samp>~/kartik $ mermaid pulse.io --hot-path</samp>

<samp>MY FAVOURITE THING I'VE BUILT — A REDIRECT THAT NEVER WAITS FOR ANALYTICS</samp>

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

<sup>The redirect and the analytics never share a thread of fate — every click enqueues a BullMQ job, background workers do the heavy lifting. <a href="https://github.com/Consoder/Pulse.io"><b>→ read the code</b></a></sup>

<br/>

<div align="center"><samp>─────── ✦ ───────</samp></div>

<!-- ════════════════════════════ SELECTED WORK ════════════════════════════ -->

## <samp>~/kartik $ ls projects/ --sort=impact</samp>

<img align="right" width="300" src="https://media.giphy.com/media/juua9i2c2fA0AIp2iq/giphy.gif" alt="dev board gif"/>

<samp>THREE BUILDS · REAL METRICS · CODE IS PUBLIC — OPEN ANY REPO AND GRILL ME ON IT.</samp>

<br clear="right"/>

<table width="100%">
<tr>
<td width="33%" valign="top">

### ⚡ Pulse.io
<samp>LINK INTELLIGENCE ENGINE</samp>

Sub-50ms redirects (architecture ↑). JWT + Google OAuth, MongoDB aggregation pipelines powering geo / device / campaign breakdowns, Recharts + Framer Motion dashboard.

`React` `Node` `Express` `MongoDB` `Redis` `BullMQ`

<kbd><a href="https://github.com/Consoder/Pulse.io">→ REPO</a></kbd>

</td>
<td width="33%" valign="top">

### 🔍 Code Analysis Platform
<samp>AI CODE REVIEW · 7 LANGUAGES</samp>

Bug detection, Big-O analysis, quality scoring. Redis cache keyed on **SHA-256 of source** — repeat analysis drops from 2–8s to **~40ms**. JWT + OAuth, rate limiting, PostgreSQL.

`Next.js 14` `FastAPI` `Redis` `PostgreSQL`

<kbd><a href="https://github.com/Consoder/ROASTCODE">→ REPO</a></kbd>

</td>
<td width="33%" valign="top">

### 🚗 Vision Navigation
<samp>BEHAVIORAL CLONING CNN</samp>

NVIDIA-style end-to-end CNN, 4,500+ labeled frames → **121K params, 94.1% val accuracy**, real-time CPU inference. Pygame sim with **Grad-CAM** overlays showing what the model watches while steering.

`Python` `TensorFlow` `OpenCV` `Pygame`

<kbd><a href="https://github.com/Consoder/Vision-Based-Autonomous-Navigation-System">→ REPO</a></kbd>

</td>
</tr>
</table>

<sub>ALSO — <a href="https://github.com/Consoder/saas-notes-app"><b>saas-notes-app</b></a> · multi-tenant API, JWT + RBAC &nbsp;/&nbsp; <a href="https://github.com/Consoder/SMS-IDENTIFIER"><b>SMS-IDENTIFIER</b></a> · TF-IDF spam classifier &nbsp;/&nbsp; <a href="https://github.com/Consoder?tab=repositories">full index →</a></sub>

<br/>

<div align="center"><samp>─────── ✦ ───────</samp></div>

<!-- ════════════════════════════ EXPERIENCE ════════════════════════════ -->

## <samp>~/kartik $ git log --experience</samp>

<img align="right" width="300" src="https://media.giphy.com/media/SWoSkN6DxTszqIKEqv/giphy.gif" alt="developer at desk gif"/>

```text
* commit 2026.05 → 2026.06  (HEAD)
│ role:    Software Engineer — Full-Stack Intern
│ org:     Wisflux Pvt. Ltd
│ work:    secure REST APIs, auth/authorization & backend features for a
│          MERN link-management platform · Agile/Scrum · code reviews ·
│          performance optimization
│
* commit 2025.05 → 2025.07
│ role:    Python & Machine Learning Intern
│ org:     KisTechno Software Pvt. Ltd
│ work:    end-to-end self-driving simulator — data collection, training,
│          evaluation → 94%+ accuracy · Grad-CAM explainability
```

<br clear="right"/>

<samp>**HONOURS**</samp> &nbsp;·&nbsp; 🥈 IEEE Hackathon — **2nd Place** (working prototype + go-to-market) &nbsp;·&nbsp; 🎤 DevOps Workshop **Coordinator** — 100+ students

<samp>**CREDENTIALS**</samp> &nbsp;·&nbsp; ☁️ AWS Cloud Practitioner Essentials &nbsp;·&nbsp; ✨ Google Vertex AI — Prompt Design &nbsp;·&nbsp; 📊 Deloitte Data Analytics

<br/>

<div align="center"><samp>─────── ✦ ───────</samp></div>

<!-- ════════════════════════════ STACK ════════════════════════════ -->

## <samp>~/kartik $ tree stack/</samp>

<div align="center">

<img src="https://skillicons.dev/icons?i=cpp,python,js,c,mysql&theme=dark"/>
<br/><br/>
<img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,express,fastapi,tailwind&theme=dark"/>
<br/><br/>
<img src="https://skillicons.dev/icons?i=postgres,mongodb,redis,docker,aws,git,github,githubactions,postman&theme=dark"/>

<br/>

<sub><samp>CORE CS — DSA · OOP · DBMS · OPERATING SYSTEMS · COMPUTER NETWORKS · REST · CI/CD</samp></sub>

</div>

<br/>

<div align="center"><samp>─────── ✦ ───────</samp></div>

<!-- ════════════════════════════ TELEMETRY ════════════════════════════ -->

## <samp>~/kartik $ htop --github</samp>

<div align="center">

<img src="https://github-profile-trophy.vercel.app/?username=Consoder&theme=radical&no-frame=true&no-bg=true&column=7&margin-w=8" width="100%"/>

<br/><br/>

<img height="165" src="https://github-readme-stats.vercel.app/api?username=Consoder&show_icons=true&hide_border=true&bg_color=0d001a&title_color=a78bfa&text_color=e8d5ff&icon_color=C9A876&ring_color=8b5cf6"/>&nbsp;<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Consoder&layout=compact&hide_border=true&bg_color=0d001a&title_color=a78bfa&text_color=e8d5ff&langs_count=8"/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Consoder&bg_color=0d001a&color=a78bfa&line=8b5cf6&point=C9A876&area=true&area_color=1a0533&hide_border=true&hide_title=true" width="100%"/>

<br/><br/>

<!-- CONTRIBUTION SNAKE — powered by .github/workflows/snake.yml in this repo -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Consoder/Consoder/output/github-contribution-grid-snake-dark.svg"/>
  <img alt="contribution snake" src="https://raw.githubusercontent.com/Consoder/Consoder/output/github-contribution-grid-snake-dark.svg"/>
</picture>

</div>

<br/>

<!-- ════════════════════════════ CONTACT ════════════════════════════ -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&height=3&color=0:C9A876,50:8b5cf6,100:C9A876" width="100%"/>

<br/><br/>

<img width="320" src="https://media.giphy.com/media/L1R1tvI9svkIWwpVYr/giphy.gif" alt="typing on laptop"/>

<br/><br/>

<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=500&size=22&duration=1&pause=99999&color=C9A876&center=true&vCenter=true&width=600&height=40&lines=Let's+build+something+real." />

<br/>

<kbd><a href="https://kartik-portfolio-6k36.vercel.app/">&nbsp;PORTFOLIO&nbsp;</a></kbd>&nbsp;&nbsp;
<kbd><a href="https://www.linkedin.com/in/kartik-bhargava-248796257">&nbsp;LINKEDIN&nbsp;</a></kbd>&nbsp;&nbsp;
<kbd><a href="mailto:kartikbhargava1111@gmail.com">&nbsp;KARTIKBHARGAVA1111@GMAIL.COM&nbsp;</a></kbd>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=Consoder&style=flat-square&color=8b5cf6&label=PROFILE+VIEWS" />

<br/><br/>

<sub><samp>© 2026 KARTIK BHARGAVA · $ exit 0</samp></sub>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=rect&height=3&color=0:C9A876,50:8b5cf6,100:C9A876" width="100%"/>

</div>
