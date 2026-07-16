<!-- ═══════════════════════════════ HERO ═══════════════════════════════ -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=220&color=0:0a0a0f,35:2a0a4a,70:4c1d95,100:0d001a&text=KARTIK%20BHARGAVA&fontSize=48&fontColor=e8d5ff&fontAlignY=38&animation=fadeIn&desc=FULL-STACK%20ENGINEER%20%C2%B7%20B.TECH%20CSE%20'27%20%C2%B7%20SKIT%20JAIPUR&descSize=14&descAlignY=58" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Great+Vibes&weight=500&size=34&duration=1&pause=99999&color=C9A876&center=true&vCenter=true&width=700&height=55&lines=Building+products+people+love+to+use" />

<img src="https://raw.githubusercontent.com/ABSphreak/ABSphreak/master/gifs/Hi.gif" width="40" alt="hi"/>&nbsp;&nbsp;
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=400&size=14&duration=2600&pause=600&color=A78BFA&center=true&vCenter=true&width=560&lines=React+%C2%B7+Next.js+%C2%B7+Node+%C2%B7+FastAPI+%C2%B7+Redis+%C2%B7+Postgres;%F0%9F%9F%A2+open+to+SDE+%2F+full-stack+%2F+backend+roles;385%2B+DSA+solved+%C2%B7+sub-50ms+systems+%C2%B7+shipping+weekly" />

<br/>

<a href="https://kartik-portfolio-6k36.vercel.app/"><img src="https://img.shields.io/badge/⌘_PORTFOLIO-1a0533?style=for-the-badge&logoColor=C9A876&labelColor=1a0533&color=8b5cf6"/></a>&nbsp;
<a href="https://www.linkedin.com/in/kartik-bhargava-248796257"><img src="https://img.shields.io/badge/LINKEDIN-1a0533?style=for-the-badge&logo=linkedin&logoColor=e8d5ff&labelColor=1a0533&color=4c1d95"/></a>&nbsp;
<a href="mailto:kartikbhargava1111@gmail.com"><img src="https://img.shields.io/badge/EMAIL-1a0533?style=for-the-badge&logo=gmail&logoColor=e8d5ff&labelColor=1a0533&color=8b5cf6"/></a>&nbsp;
<a href="https://github.com/Consoder?tab=repositories"><img src="https://img.shields.io/badge/ALL_REPOS-1a0533?style=for-the-badge&logo=github&logoColor=e8d5ff&labelColor=1a0533&color=4c1d95"/></a>

</div>

<br/>

<!-- ═══════════════════════════════ 01 ABOUT ═══════════════════════════════ -->

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=600&size=26&duration=1&pause=99999&color=E8D5FF&center=true&vCenter=true&width=420&height=42&lines=01+%E2%80%94+The+Engineer" />
<img src="https://capsule-render.vercel.app/api?type=rect&height=2&color=0:C9A876,50:8b5cf6,100:C9A876" width="42%"/>
</div>

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

<!-- ═══════════════════════════════ 02 ARCHITECTURE ═══════════════════════════════ -->

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=600&size=26&duration=1&pause=99999&color=E8D5FF&center=true&vCenter=true&width=480&height=42&lines=02+%E2%80%94+Architecture+I'm+Proud+Of" />
<img src="https://capsule-render.vercel.app/api?type=rect&height=2&color=0:C9A876,50:8b5cf6,100:C9A876" width="42%"/>
<br/><br/>
<samp>PULSE.IO — A REDIRECT THAT NEVER WAITS FOR ANALYTICS</samp>
</div>

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

<div align="center"><sup>Every click enqueues a BullMQ job — background workers do the heavy lifting, the redirect never blocks. <a href="https://github.com/Consoder/Pulse.io"><b>→ read the code</b></a></sup></div>

<br/>

<!-- ═══════════════════════════════ 03 PROJECTS ═══════════════════════════════ -->

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=600&size=26&duration=1&pause=99999&color=E8D5FF&center=true&vCenter=true&width=420&height=42&lines=03+%E2%80%94+Selected+Work" />
<img src="https://capsule-render.vercel.app/api?type=rect&height=2&color=0:C9A876,50:8b5cf6,100:C9A876" width="42%"/>
</div>

<table width="100%">
<tr>
<td width="33%" valign="top" align="center">

<h3>⚡ Pulse.io</h3>
<samp>LINK INTELLIGENCE ENGINE</samp>

<p align="left">Sub-50ms redirects (architecture ↑). JWT + Google OAuth, MongoDB aggregation pipelines for geo / device / campaign breakdowns, Recharts + Framer Motion dashboard.</p>

<img src="https://img.shields.io/badge/React-1a0533?style=flat-square&logo=react&logoColor=a78bfa"/> <img src="https://img.shields.io/badge/Node-1a0533?style=flat-square&logo=nodedotjs&logoColor=a78bfa"/> <img src="https://img.shields.io/badge/MongoDB-1a0533?style=flat-square&logo=mongodb&logoColor=a78bfa"/> <img src="https://img.shields.io/badge/Redis-1a0533?style=flat-square&logo=redis&logoColor=a78bfa"/> <img src="https://img.shields.io/badge/BullMQ-1a0533?style=flat-square&logoColor=a78bfa"/>

<a href="https://github.com/Consoder/Pulse.io"><img src="https://img.shields.io/badge/→_REPOSITORY-C9A876?style=for-the-badge&labelColor=1a0533&color=1a0533&logoColor=C9A876"/></a>

</td>
<td width="33%" valign="top" align="center">

<h3>🔍 Code Analysis Platform</h3>
<samp>AI CODE REVIEW · 7 LANGUAGES</samp>

<p align="left">Bug detection, Big-O analysis, quality scoring. Redis cache keyed on <b>SHA-256 of source</b> — repeat analysis drops from 2–8s to <b>~40ms</b>. JWT + OAuth, rate limiting, PostgreSQL.</p>

<img src="https://img.shields.io/badge/Next.js_14-1a0533?style=flat-square&logo=nextdotjs&logoColor=a78bfa"/> <img src="https://img.shields.io/badge/FastAPI-1a0533?style=flat-square&logo=fastapi&logoColor=a78bfa"/> <img src="https://img.shields.io/badge/Redis-1a0533?style=flat-square&logo=redis&logoColor=a78bfa"/> <img src="https://img.shields.io/badge/PostgreSQL-1a0533?style=flat-square&logo=postgresql&logoColor=a78bfa"/>

<a href="https://github.com/Consoder/ROASTCODE"><img src="https://img.shields.io/badge/→_REPOSITORY-C9A876?style=for-the-badge&labelColor=1a0533&color=1a0533&logoColor=C9A876"/></a>

</td>
<td width="33%" valign="top" align="center">

<h3>🚗 Vision Navigation</h3>
<samp>BEHAVIORAL CLONING CNN</samp>

<p align="left">NVIDIA-style end-to-end CNN, 4,500+ labeled frames → <b>121K params, 94.1% val accuracy</b>, real-time CPU inference. Pygame sim with <b>Grad-CAM</b> showing what the model watches while steering.</p>

<img src="https://img.shields.io/badge/Python-1a0533?style=flat-square&logo=python&logoColor=a78bfa"/> <img src="https://img.shields.io/badge/TensorFlow-1a0533?style=flat-square&logo=tensorflow&logoColor=a78bfa"/> <img src="https://img.shields.io/badge/OpenCV-1a0533?style=flat-square&logo=opencv&logoColor=a78bfa"/> <img src="https://img.shields.io/badge/Pygame-1a0533?style=flat-square&logoColor=a78bfa"/>

<a href="https://github.com/Consoder/Vision-Based-Autonomous-Navigation-System"><img src="https://img.shields.io/badge/→_REPOSITORY-C9A876?style=for-the-badge&labelColor=1a0533&color=1a0533&logoColor=C9A876"/></a>

</td>
</tr>
</table>

<div align="center"><sub>ALSO — <a href="https://github.com/Consoder/saas-notes-app"><b>saas-notes-app</b></a> · multi-tenant API, JWT + RBAC &nbsp;/&nbsp; <a href="https://github.com/Consoder/SMS-IDENTIFIER"><b>SMS-IDENTIFIER</b></a> · TF-IDF spam classifier</sub></div>

<br/>

<!-- ═══════════════════════════════ 04 EXPERIENCE ═══════════════════════════════ -->

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=600&size=26&duration=1&pause=99999&color=E8D5FF&center=true&vCenter=true&width=420&height=42&lines=04+%E2%80%94+Experience" />
<img src="https://capsule-render.vercel.app/api?type=rect&height=2&color=0:C9A876,50:8b5cf6,100:C9A876" width="42%"/>
</div>

<table width="100%">
<tr>
<td width="26%" align="center" valign="middle">

<img src="https://img.shields.io/badge/MAY–JUN_2026-1a0533?style=for-the-badge&color=4c1d95"/>

</td>
<td width="74%" valign="middle">

<b>Software Engineer — Full-Stack Intern</b> · Wisflux Pvt. Ltd<br/>
<sub>Secure REST APIs, auth/authorization & backend features for a scalable MERN link-management platform · Agile/Scrum · code reviews · performance optimization</sub>

</td>
</tr>
<tr>
<td width="26%" align="center" valign="middle">

<img src="https://img.shields.io/badge/MAY–JUL_2025-1a0533?style=for-the-badge&color=4c1d95"/>

</td>
<td width="74%" valign="middle">

<b>Python & Machine Learning Intern</b> · KisTechno Software Pvt. Ltd<br/>
<sub>End-to-end self-driving simulator — data collection, training, evaluation → 94%+ accuracy · Grad-CAM explainability added on mentor feedback</sub>

</td>
</tr>
</table>

<table width="100%">
<tr>
<td width="50%" align="center" valign="top">

<samp>🏆 HONOURS</samp><br/><br/>
🥈 IEEE Hackathon — <b>2nd Place</b><br/><sub>working prototype + go-to-market strategy</sub><br/><br/>
🎤 DevOps Workshop <b>Coordinator</b><br/><sub>100+ students</sub>

</td>
<td width="50%" align="center" valign="top">

<samp>📜 CREDENTIALS</samp><br/><br/>
☁️ AWS Cloud Practitioner Essentials<br/><sub>EC2 · S3 · VPC · IAM</sub><br/><br/>
✨ Google Vertex AI — Prompt Design &nbsp;·&nbsp; 📊 Deloitte Data Analytics

</td>
</tr>
</table>

<br/>

<!-- ═══════════════════════════════ 05 STACK ═══════════════════════════════ -->

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=600&size=26&duration=1&pause=99999&color=E8D5FF&center=true&vCenter=true&width=420&height=42&lines=05+%E2%80%94+The+Stack" />
<img src="https://capsule-render.vercel.app/api?type=rect&height=2&color=0:C9A876,50:8b5cf6,100:C9A876" width="42%"/>
</div>

<table width="100%">
<tr>
<td align="center" width="20%"><samp>LANGUAGES</samp></td>
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
<td align="center"><samp>TOOLS ×<br/>CLOUD</samp></td>
<td align="center"><img src="https://skillicons.dev/icons?i=git,github,githubactions,docker,aws,postman&theme=dark"/></td>
</tr>
</table>

<div align="center"><sub><samp>CORE CS — DSA · OOP · DBMS · OPERATING SYSTEMS · COMPUTER NETWORKS · REST · CI/CD</samp></sub></div>

<br/>

<!-- ═══════════════════════════════ 06 TELEMETRY ═══════════════════════════════ -->

<div align="center">
<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=600&size=26&duration=1&pause=99999&color=E8D5FF&center=true&vCenter=true&width=420&height=42&lines=06+%E2%80%94+Telemetry" />
<img src="https://capsule-render.vercel.app/api?type=rect&height=2&color=0:C9A876,50:8b5cf6,100:C9A876" width="42%"/>

<br/><br/>

<img src="https://github-profile-trophy.vercel.app/?username=Consoder&theme=radical&no-frame=true&no-bg=true&column=7&margin-w=8" width="100%"/>

<br/><br/>

<img height="165" src="https://github-readme-stats.vercel.app/api?username=Consoder&show_icons=true&hide_border=true&bg_color=0d001a&title_color=a78bfa&text_color=e8d5ff&icon_color=C9A876&ring_color=8b5cf6"/>&nbsp;<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Consoder&layout=compact&hide_border=true&bg_color=0d001a&title_color=a78bfa&text_color=e8d5ff&langs_count=8"/>

<br/><br/>

<!-- CONTRIBUTION SNAKE — powered by .github/workflows/snake.yml -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Consoder/Consoder/output/github-contribution-grid-snake-dark.svg"/>
  <img alt="contribution snake" src="https://raw.githubusercontent.com/Consoder/Consoder/output/github-contribution-grid-snake-dark.svg"/>
</picture>

</div>

<br/>

<!-- ═══════════════════════════════ CONTACT ═══════════════════════════════ -->

<div align="center">

<img src="https://media.giphy.com/media/L1R1tvI9svkIWwpVYr/giphy.gif" width="300" alt="typing"/>

<img src="https://readme-typing-svg.demolab.com?font=Great+Vibes&weight=500&size=30&duration=1&pause=99999&color=C9A876&center=true&vCenter=true&width=600&height=50&lines=Let's+build+something+real" />

<a href="https://kartik-portfolio-6k36.vercel.app/"><img src="https://img.shields.io/badge/⌘_PORTFOLIO-1a0533?style=for-the-badge&labelColor=1a0533&color=8b5cf6"/></a>&nbsp;
<a href="https://www.linkedin.com/in/kartik-bhargava-248796257"><img src="https://img.shields.io/badge/LINKEDIN-1a0533?style=for-the-badge&logo=linkedin&logoColor=e8d5ff&labelColor=1a0533&color=4c1d95"/></a>&nbsp;
<a href="mailto:kartikbhargava1111@gmail.com"><img src="https://img.shields.io/badge/EMAIL-1a0533?style=for-the-badge&logo=gmail&logoColor=e8d5ff&labelColor=1a0533&color=8b5cf6"/></a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=Consoder&style=for-the-badge&color=8b5cf6&label=PROFILE+VIEWS" />

<img src="https://capsule-render.vercel.app/api?type=waving&height=130&color=0:0d001a,50:4c1d95,100:0a0a0f&section=footer&text=BUILD%20FAST.%20SHIP%20CLEAN.%20MAKE%20IT%20REAL.&fontSize=15&fontColor=C9A876&fontAlignY=78" width="100%"/>

</div>
