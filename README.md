<!--
  TYPE SYSTEM — Google Fonts, rendered server-side as SVG images.
  (GitHub strips <link> and <style>, so SVG text is the only way to ship a real font.)

  Playfair Display 700 ... headings only (name + section headers)
  Cinzel 600 ............. every other styleable text
  (Body paragraphs fall back to GitHub's default face — markdown text cannot be styled.)

  COLOR ROLES
  #C9A876 gold ....... section headers
  #E8D5FF lavender ... name + card titles
  #A78BFA violet ..... supporting / mono text
  #1a0533 indigo ..... badge fills

  LOCAL ASSETS (repo root)
  hero-terminal_1.gif · matrix-rain.gif · footer-terminal.gif · divider.gif
-->

<table width="100%">
<tr>
<td width="440" align="center" valign="middle">

<img src="https://raw.githubusercontent.com/Consoder/Consoder/main/hero-terminal_1.gif" width="420" alt="Kartik Bhargava — ASCII portrait decoding in a terminal"/>

</td>
<td width="440" align="center" valign="middle">

<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=700&size=40&duration=1&pause=99999&color=E8D5FF&center=true&vCenter=true&width=420&height=66&lines=Kartik+Bhargava" alt="Kartik Bhargava"/>

<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=15&duration=1&pause=99999&color=A78BFA&center=true&vCenter=true&width=420&height=36&lines=Full-Stack+%C2%B7+Backend+Engineer" alt="Full-Stack · Backend Engineer"/>

<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=13&duration=1&pause=99999&color=C9A876&center=true&vCenter=true&width=420&height=32&lines=Open+to+SDE+%2F+Full-Stack+%2F+Backend+%C2%B7+Remote-Ready" alt="Open to SDE / Full-Stack / Backend · Remote-Ready"/>

<br/>

<img src="https://skillicons.dev/icons?i=cpp,python,js,typescript,react,nextjs&theme=dark&perline=6" height="38"/>

<img src="https://skillicons.dev/icons?i=nodejs,express,fastapi,postgres,mongodb,redis&theme=dark&perline=6" height="38"/>

<img src="https://skillicons.dev/icons?i=docker,aws,githubactions,git,tailwind,postman&theme=dark&perline=6" height="38"/>

<br/><br/>

<a href="https://kartik-portfolio-6k36.vercel.app/"><img src="https://img.shields.io/badge/PORTFOLIO-1a0533?style=flat-square&labelColor=1a0533&color=1a0533&logo=vercel&logoColor=C9A876" height="28"/></a>&nbsp;
<a href="https://www.linkedin.com/in/kartik-bhargava-248796257"><img src="https://img.shields.io/badge/LINKEDIN-1a0533?style=flat-square&labelColor=1a0533&color=1a0533&logo=linkedin&logoColor=a78bfa" height="28"/></a>&nbsp;
<a href="mailto:kartikbhargava1111@gmail.com"><img src="https://img.shields.io/badge/EMAIL-1a0533?style=flat-square&labelColor=1a0533&color=1a0533&logo=gmail&logoColor=a78bfa" height="28"/></a>&nbsp;
<a href="https://github.com/Consoder?tab=repositories"><img src="https://img.shields.io/badge/REPOS-1a0533?style=flat-square&labelColor=1a0533&color=1a0533&logo=github&logoColor=a78bfa" height="28"/></a>

</td>
</tr>
</table>

<img src="https://raw.githubusercontent.com/Consoder/Consoder/main/divider.gif" width="100%" alt=""/>

<br/>

<!-- ═════════════════════ 01 — THE ENGINEER ═════════════════════ -->

<h2>
<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=700&size=27&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=420&height=44&lines=01.+The+Engineer" alt="01. The Engineer"/>
</h2>

<table width="100%">
<tr>
<td width="500" valign="top">

```typescript
const kartik = {
  remote: true,
  education: "B.Tech CSE '27 · SKIT · 8.3 CGPA",

  languages: ["C++", "Python", "JavaScript", "SQL", "C"],
  backend:   ["Node", "Express", "FastAPI"],
  frontend:  ["React", "Next.js", "Tailwind"],
  data:      ["PostgreSQL", "MongoDB", "Redis"],
  infra:     ["Docker", "AWS", "GitHub Actions"],

  obsession: "systems where the hot path never blocks",
  hireable: true,
};
```

</td>
<td width="380" align="center" valign="middle">
<img src="https://raw.githubusercontent.com/Consoder/Consoder/main/matrix-rain.gif" width="360" alt="digital rain"/>
</td>
</tr>
</table>

<img src="https://raw.githubusercontent.com/Consoder/Consoder/main/divider.gif" width="100%" alt=""/>

<br/>

<!-- ═════════════════════ 02 — THE ARCHITECTURE ═════════════════════ -->

<h2>
<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=700&size=27&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=460&height=44&lines=02.+The+Architecture" alt="02. The Architecture"/>
</h2>

<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=14&duration=1&pause=99999&color=A78BFA&center=false&vCenter=true&width=620&height=28&lines=Pulse.io+%E2%80%94+a+redirect+that+never+waits+for+analytics" alt="Pulse.io — a redirect that never waits for analytics"/>

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

<sub>Every click enqueues a BullMQ job — workers do the heavy lifting off the hot path, so the redirect never waits for analytics. <a href="https://github.com/Consoder/Pulse.io"><b>→ read the code</b></a></sub>

<br/><br/>

<img src="https://raw.githubusercontent.com/Consoder/Consoder/main/divider.gif" width="100%" alt=""/>

<br/>

<!-- ═════════════════════ 03 — SELECTED WORKS ═════════════════════ -->

<h2>
<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=700&size=27&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=460&height=44&lines=03.+Selected+Works" alt="03. Selected Works"/>
</h2>

<table width="100%">
<tr>
<td width="293" valign="top">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=12&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=280&height=24&lines=Link+Intelligence+Engine" alt="Link Intelligence Engine"/>
<h3>⚡ Pulse.io</h3>
Sub-50ms redirects. JWT + Google OAuth, MongoDB aggregation pipelines for geo / device / campaign breakdowns, Recharts + Framer Motion dashboard.
<br/><br/>
<code>React</code> <code>Node</code> <code>Express</code> <code>MongoDB</code> <code>Redis</code> <code>BullMQ</code>
<br/><br/>
<a href="https://github.com/Consoder/Pulse.io"><b>→ repository</b></a>
</td>
<td width="293" valign="top">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=12&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=280&height=24&lines=AI+Code+Review+%C2%B7+7+Languages" alt="AI Code Review · 7 Languages"/>
<h3>🔍 Code Analysis Platform</h3>
Bug detection, Big-O analysis, quality scoring. Redis cache keyed on SHA-256 of source — repeat analysis drops from 2–8s to <b>~40ms</b>. JWT + OAuth, rate limiting.
<br/><br/>
<code>Next.js 14</code> <code>FastAPI</code> <code>Redis</code> <code>PostgreSQL</code>
<br/><br/>
<a href="https://github.com/Consoder/ROASTCODE"><b>→ repository</b></a>
</td>
<td width="293" valign="top">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=12&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=280&height=24&lines=Behavioral+Cloning+CNN" alt="Behavioral Cloning CNN"/>
<h3>🚗 Vision Navigation</h3>
NVIDIA-style end-to-end CNN, 4,500+ labeled frames → <b>121K params, 94.1% val accuracy</b>, real-time CPU inference. Pygame sim with Grad-CAM overlays.
<br/><br/>
<code>Python</code> <code>TensorFlow</code> <code>OpenCV</code> <code>Pygame</code>
<br/><br/>
<a href="https://github.com/Consoder/Vision-Based-Autonomous-Navigation-System"><b>→ repository</b></a>
</td>
</tr>
</table>

<sub>ALSO — <a href="https://github.com/Consoder/saas-notes-app"><b>saas-notes-app</b></a> · multi-tenant API, JWT + RBAC &nbsp;·&nbsp; <a href="https://github.com/Consoder/SMS-IDENTIFIER"><b>SMS-IDENTIFIER</b></a> · TF-IDF spam classifier</sub>

<br/><br/>

<img src="https://raw.githubusercontent.com/Consoder/Consoder/main/divider.gif" width="100%" alt=""/>

<br/>

<!-- ═════════════════════ 04 — THE EXPERIENCE ═════════════════════ -->

<h2>
<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=700&size=27&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=460&height=44&lines=04.+The+Experience" alt="04. The Experience"/>
</h2>

<table width="100%">
<tr>
<td width="150" align="center" valign="middle">
<img src="https://img.shields.io/badge/MAY_–_JUN_2026-1a0533?style=flat-square&labelColor=1a0533&color=1a0533"/>
</td>
<td width="730" valign="middle">
<b>Software Engineer — Full-Stack Intern</b> · Wisflux Pvt. Ltd<br/>
<sub>Secure REST APIs, auth/authorization & backend features for a scalable MERN link-management platform · Agile/Scrum · code reviews · performance optimization</sub>
</td>
</tr>
<tr><td colspan="2" height="14"></td></tr>
<tr>
<td width="150" align="center" valign="middle">
<img src="https://img.shields.io/badge/MAY_–_JUL_2025-1a0533?style=flat-square&labelColor=1a0533&color=1a0533"/>
</td>
<td width="730" valign="middle">
<b>Python & Machine Learning Intern</b> · KisTechno Software Pvt. Ltd<br/>
<sub>End-to-end self-driving simulator — data collection, training, evaluation → 94%+ accuracy · Grad-CAM explainability added on mentor feedback</sub>
</td>
</tr>
</table>

<br/>

<table width="100%">
<tr>
<td width="60" align="center" valign="middle">🏅</td>
<td width="380" valign="middle">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=15&duration=1&pause=99999&color=E8D5FF&center=false&vCenter=true&width=340&height=28&lines=HackerRank" alt="HackerRank SQL Certified"/><br/>
<b>Advanced Certified</b><br/><sub>Verified advanced-level assessment</sub>
</td>
<td width="60" align="center" valign="middle">☁️</td>
<td width="380" valign="middle">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=15&duration=1&pause=99999&color=E8D5FF&center=false&vCenter=true&width=340&height=28&lines=AWS+Certified" alt="AWS Certified"/><br/>
<b>Cloud Practitioner Essentials</b><br/><sub>EC2 · S3 · VPC · IAM</sub>
</td>
</tr>
<tr><td colspan="4" height="18"></td></tr>
<tr>
<td width="60" align="center" valign="middle">🥈</td>
<td width="380" valign="middle">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=15&duration=1&pause=99999&color=E8D5FF&center=false&vCenter=true&width=340&height=28&lines=IEEE+Hackathon" alt="IEEE Hackathon"/><br/>
<b>2nd Place</b><br/><sub>Working prototype + go-to-market strategy</sub>
</td>
<td width="60" align="center" valign="middle">🎤</td>
<td width="380" valign="middle">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=15&duration=1&pause=99999&color=E8D5FF&center=false&vCenter=true&width=340&height=28&lines=DevOps+Workshop" alt="DevOps Workshop"/><br/>
<b>Coordinator</b><br/><sub>Led a session for 100+ students</sub>
</td>
</tr>
<tr><td colspan="4" height="18"></td></tr>
<tr>
<td width="60" align="center" valign="middle">✨</td>
<td width="380" valign="middle">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=15&duration=1&pause=99999&color=E8D5FF&center=false&vCenter=true&width=340&height=28&lines=Google+Vertex+AI" alt="Google Vertex AI"/><br/>
<b>Prompt Design</b><br/><sub>Generative AI track</sub>
</td>
<td width="60" align="center" valign="middle">📊</td>
<td width="380" valign="middle">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=15&duration=1&pause=99999&color=E8D5FF&center=false&vCenter=true&width=340&height=28&lines=Deloitte" alt="Deloitte"/><br/>
<b>Data Analytics</b><br/><sub>Job simulation programme</sub>
</td>
</tr>
</table>

<img src="https://raw.githubusercontent.com/Consoder/Consoder/main/divider.gif" width="100%" alt=""/>

<br/>

<!-- ═════════════════════ 05 — THE STACK ═════════════════════ -->

<h2>
<img src="https://readme-typing-svg.demolab.com?font=Playfair+Display&weight=700&size=27&duration=1&pause=99999&color=C9A876&center=false&vCenter=true&width=420&height=44&lines=05.+The+Stack" alt="05. The Stack"/>
</h2>

<table width="100%">
<tr>
<td width="180" valign="middle">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=14&duration=1&pause=99999&color=A78BFA&center=false&vCenter=true&width=170&height=26&lines=Languages" alt="Languages"/>
</td>
<td width="700" valign="middle">
<img src="https://skillicons.dev/icons?i=cpp,python,js,c,mysql&theme=dark&perline=8" height="52"/>
</td>
</tr>
<tr><td colspan="2" height="12"></td></tr>
<tr>
<td width="180" valign="middle">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=14&duration=1&pause=99999&color=A78BFA&center=false&vCenter=true&width=170&height=26&lines=Front+%2B+Back" alt="Front + Back"/>
</td>
<td width="700" valign="middle">
<img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,express,fastapi,tailwind&theme=dark&perline=8" height="52"/>
</td>
</tr>
<tr><td colspan="2" height="12"></td></tr>
<tr>
<td width="180" valign="middle">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=14&duration=1&pause=99999&color=A78BFA&center=false&vCenter=true&width=170&height=26&lines=Data" alt="Data"/>
</td>
<td width="700" valign="middle">
<img src="https://skillicons.dev/icons?i=postgres,mongodb,redis&theme=dark&perline=8" height="52"/>
</td>
</tr>
<tr><td colspan="2" height="12"></td></tr>
<tr>
<td width="180" valign="middle">
<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=600&size=14&duration=1&pause=99999&color=A78BFA&center=false&vCenter=true&width=170&height=26&lines=Tools+%2B+Cloud" alt="Tools + Cloud"/>
</td>
<td width="700" valign="middle">
<img src="https://skillicons.dev/icons?i=git,github,githubactions,docker,aws,postman&theme=dark&perline=8" height="52"/>
</td>
</tr>
</table>

<sub>CORE CS — DSA · OOP · DBMS · Operating Systems · Computer Networks · REST · CI/CD</sub>

<br/><br/>

<img src="https://raw.githubusercontent.com/Consoder/Consoder/main/divider.gif" width="100%" alt=""/>

<br/>

<!-- ═════════════════════ SIGN-OFF ═════════════════════ -->

<div align="center">

<img src="https://raw.githubusercontent.com/Consoder/Consoder/main/footer-terminal.gif" width="880" alt="kartik@dev — contact card"/>

<br/><br/>

<a href="https://kartik-portfolio-6k36.vercel.app/"><img src="https://img.shields.io/badge/PORTFOLIO-1a0533?style=flat-square&labelColor=1a0533&color=1a0533&logo=vercel&logoColor=C9A876" height="28"/></a>&nbsp;
<a href="https://www.linkedin.com/in/kartik-bhargava-248796257"><img src="https://img.shields.io/badge/LINKEDIN-1a0533?style=flat-square&labelColor=1a0533&color=1a0533&logo=linkedin&logoColor=a78bfa" height="28"/></a>&nbsp;
<a href="mailto:kartikbhargava1111@gmail.com"><img src="https://img.shields.io/badge/EMAIL-1a0533?style=flat-square&labelColor=1a0533&color=1a0533&logo=gmail&logoColor=a78bfa" height="28"/></a>

</div>
