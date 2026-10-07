<!-- Repo name must be exactly: anirudhkrishna-06/anirudhkrishna-06 -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Anirudh%20Krishna%20M&fontSize=46&fontColor=ffffff&fontAlignY=38&desc=Builds%20systems%20that%20keep%20time%20%E2%80%94%20in%20code%20and%20on%20the%20mridangam&descSize=16&descAlignY=60" width="100%" alt="banner" />

<a href="https://github.com/anirudhkrishna-06">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=00E5FF&center=true&vCenter=true&width=700&lines=SDE+Intern+%40+Amazon;Building+a+distributed+KV+store+from+scratch+in+Go;Making+LLM+output+reliable%2C+not+just+impressive;Department+Rank+1+%7C+CGPA+8.99+%7C+SSN+College%2C+Chennai" alt="typing animation" />
</a>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/anirudhkrishna06)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/abrokecollegeguy/)
[![Portfolio](https://img.shields.io/badge/Portfolio-0f2027?style=for-the-badge&logo=vercel&logoColor=white)](https://anirudhkrishna-portfolio.netlify.app/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:anikrishofficial@gmail.com)

</div>

<br/>

<div align="center">
  <img src="assets/profile-card.svg" width="100%" alt="Anirudh Krishna M - terminal profile card" />
</div>

---

## 👋 Hey, I'm Anirudh

Final-year **B.Tech IT** student at **SSN College of Engineering, Chennai**, and an engineer who likes understanding *why* things work before using them. This summer I interned at **Amazon** as an SDE on a payments microservice, where correctness isn't optional. Outside work, I build databases from scratch, teach LLMs to be less confidently wrong, and play the **mridangam** professionally.

> 🥁 In Carnatic music, you keep the *tala* (the rhythm cycle) no matter how wild the improvisation gets.
> Good systems work the same way: a steady core, with room to improvise on top.

---

## 🎼 My Work, Arranged Like a Concert

Carnatic concerts have a structure. So does my work.

| Part of the concert | What it means | In my world |
|---|---|---|
| **Varnam** (the warm-up) | Fundamentals, drilled until they're muscle memory | 300+ LeetCode problems, DSA, OOD, database systems |
| **Kriti** (the main piece) | The composition that carries the show | Production-minded backend work: Java, Spring Boot, AWS |
| **Manodharma** (improvisation) | Creative exploration within rules | Agentic AI, RAG, and multi-agent planning experiments |
| **Tani Avartanam** (the solo) | Percussion takes center stage | Building a storage engine in Go, from the WAL up |

---

## 🔭 What I'm Building Right Now

### 🗄️ AtlasKV: a distributed key-value store from scratch
`Go` · `gRPC` · `Protocol Buffers` · `Raft` · `LSM Trees`

No database library, just first principles: **write-ahead log → MemTable → SSTables → compaction → crash recovery**, then consistent-hash partitioning and replication across 3–5 nodes, with an existing Raft library handling leader election and log replication.

```mermaid
flowchart LR
    C(["Client"]) -->|"gRPC"| R{"Consistent-hash router"}
    R --> N1["Node 1 - Leader"]
    R --> N2["Node 2"]
    R --> N3["Node 3"]
    N1 <-->|"Raft replication"| N2
    N1 <-->|"Raft replication"| N3
    N1 -.-> W
    subgraph SE["Storage engine per node"]
        W["WAL"] --> M["MemTable"] --> S["SSTables"] --> K["Compaction"]
    end
```

---

## 🚀 Projects

### 🧭 Routivity: geo-temporal agentic route intelligence
`Python` · `React Native` · `Firebase`

A multi-agent travel planner that thinks backwards. It **reverse-plans** from a fixed arrival time to work out when you should leave, factoring in route time, meal windows and restaurant scores, then adapts mid-route using weather and location signals. (Tested on a simulated 320 km, four-segment Chennai to Kancheepuram trip.)

```mermaid
flowchart LR
    P["Plan"] --> A["Act"] --> O["Observe"] --> F["Reflect"] --> RP["Replan"]
    RP --> A
```

### 🧮 Calcmate: structure-aware AI for math learning
`Python` · `DSPy` · `RAG` · `LLMs` · `Reinforcement Learning`

A math tutor that doesn't just *chat* about math. It turns word problems into symbolic equations and solution graphs, so LLM reasoning is grounded in deterministic computation. Each student step is validated against the graph to pinpoint exactly where a misconception begins, and an RL-based engine finds weak spots to drive adaptive quizzes.

---

## 💼 Experience

**Amazon · Software Development Engineer Intern** · May 2026 – Jul 2026 · Chennai
- Built agentic AI tools for code-review assistance, documentation maintenance and engineer onboarding on a payments microservice, delivering all 6 planned deliverables, including 2 stretch goals
- Designed a pointer-based agent memory layer to prevent data drift, informed by a study of 15+ production agents
- Raised test coverage on target components from ~35% to 95%+ and completed 21+ code reviews
- Built an on-call triage system and root-caused security defects using CloudWatch logs and git history

---

## 🛠️ Toolbox

<div align="center">

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native-0A7EA4?style=for-the-badge&logo=react&logoColor=white)

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

![gRPC](https://img.shields.io/badge/gRPC-244c5a?style=for-the-badge&logo=grpc&logoColor=white)
![DSPy](https://img.shields.io/badge/DSPy-7B2FF7?style=for-the-badge)
![RAG](https://img.shields.io/badge/RAG-FF6F00?style=for-the-badge)
![Agentic AI](https://img.shields.io/badge/Agentic_AI-0f2027?style=for-the-badge)

</div>

**AWS in practice:** CDK · CloudWatch · DynamoDB · Lambda  
**Core CS:** Data Structures & Algorithms · Database Systems · Object-Oriented Design · System Design

---

## 📊 By the Numbers

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=anirudhkrishna-06&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub stats" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=anirudhkrishna-06&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages" />

<img src="https://streak-stats.demolab.com?user=anirudhkrishna-06&theme=tokyonight&hide_border=true" alt="GitHub streak" />

<a href="https://leetcode.com/u/abrokecollegeguy/">
  <img src="https://leetcard.jacoblin.cool/abrokecollegeguy?theme=dark&font=Fira%20Code&ext=heatmap" alt="LeetCode stats" />
</a>

</div>

---

## 🏆 Beyond the Code

- 🥇 **Department Rank 1** (current), B.Tech IT, CGPA 8.99/10
- 🏁 **Smart India Hackathon**: represented my college in 2024 and 2025
- 👁️ **Head of Pixel Perception** (Computer Vision Club): led a 12-member team and technical events with 60+ attendees
- 🥁 **Professional Carnatic mridangist** with 10+ concerts

---

## 💬 Let's Talk

Always up for conversations about **distributed systems, storage engines, agentic AI, or Carnatic rhythm**, and how they're weirdly similar.

<div align="center">

📬 **anikrishofficial@gmail.com** · 📍 Chennai, India

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=100&section=footer" width="100%" alt="footer" />

</div>
