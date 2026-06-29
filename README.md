<div align="center">

<img src="header.svg" alt="kunaal" width="100%" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/kunaal-lala)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:urfav.kunaal@gmail.com)

</div>

---

**Software developer** based in Kerala, India. I build tools that eliminate friction — GPU migration pipelines, food-waste redistribution platforms, CRM automation. Working mostly solo. Learning faster than I'm comfortable with. That's the goal.

> Open to internships and collaborations — [reach out](mailto:urfav.kunaal@gmail.com)

---

## cuda-migrator

> *CUDA lock-in is just NVIDIA's way of saying "please don't leave." This tool says bye.*

**[cuda-migrator](https://github.com/kunaalxoxo/cuda-migrator)** migrates `.cu` CUDA code to AMD ROCm/HIP automatically — what used to take 2–4 weeks of engineering time now takes about 12 seconds.

```
.cu → AST parse → 65 deterministic rules → hipcc validate → MI300x benchmark → report
```

- No regex. Tree-sitter AST analysis, not grep-and-pray
- 65 transformation rules across headers, memory API, streams, events, enums
- LLM fallback via DeepSeek R1 (OpenRouter) — only for edge cases, compile-validated; hallucinations get auto-rejected
- Runs in 3 modes: stub (no AMD hardware needed), local hipcc, AMD Developer Cloud MI300x

| kernel | status | rules fired | throughput delta |
|--------|--------|-------------|------------------|
| softmax.cu | ✅ pass | 21 | +3.2% on MI300x |
| gemm.cu | ✅ pass | 15 | +1.8% on MI300x |
| attention.cu | ⚠️ warn (intentional) | 19 | +2.1% on MI300x |

AMD MI300x is 30–40% cheaper per FLOP than H100. The only thing stopping enterprises from switching is ~3 million production CUDA kernels. That's the gap this fills.

**[→ repo](https://github.com/kunaalxoxo/cuda-migrator)**

---

## platepulse

**[platepulse](https://github.com/kunaalxoxo/platepulse)** is a smart food waste redistribution platform — connects restaurants and food businesses with surplus inventory to NGOs and non-profits, so food gets used instead of thrown away.

**Stack:** React 18 + Vite, Node.js, Express, MongoDB Atlas, Redis, Socket.io

- Real-time listings and live status updates via Socket.io
- Matching logic between food donors and recipient NGOs
- Built to make the food-to-NGO handoff as frictionless as possible — zero manual coordination

**[→ repo](https://github.com/kunaalxoxo/platepulse)**

---

## what i know

```python
kunaal = {
    "ai_ml":     ["llm tooling", "python", "numpy", "pandas", "scikit-learn"],
    "systems":   ["cuda → rocm migration", "tree-sitter ast", "gpu benchmarking"],
    "crm":       ["zoho crm", "zoho people", "deluge scripting", "workflow automation"],
    "fullstack": ["react", "node.js", "express", "vue.js", "tailwind", "mongodb", "redis"],
    "devops":    ["docker", "vercel", "netlify", "render"],
    "currently": ["gsoc 2026", "open source contributions", "shipping things people actually use"],
    "fun_fact":  "built cuda-migrator in one sitting. commit timestamps are evidence.",
}
```

---

## currently building / learning

- 🔭 Exploring open source contributions for **GSoC 2026**
- 🌱 Deepening knowledge in **LLM tooling**, **compiler design**, and **GPU compute**
- ⚡ Automating everything annoying with **Deluge + Zoho** at work
- 📬 Always open to interesting problems — [kunaal.lala@outlook.com](mailto:kunaal.lala@outlook.com)

---

## other stuff that runs

| project | what it is | link |
|---------|------------|------|
| todo list app | yes everyone builds one. mine deploys and stays up | [→](https://todo-list-app-zj31.onrender.com) |
| news aggregator | real-time feed — doom-scrolling with structure | [→](https://news-aggregator-4mvu.onrender.com) |
| notes app | clean markdown notes, nothing fancy | [→](https://dynamic-kelpie-90b880.netlify.app/) |

---

## stack

**languages**

![Python](https://img.shields.io/badge/Python-3670A0?style=flat-square&logo=python&logoColor=ffdd54)
![JavaScript](https://img.shields.io/badge/JavaScript-%23323330.svg?style=flat-square&logo=javascript&logoColor=%23F7DF1E)
![C++](https://img.shields.io/badge/C++-%2300599C.svg?style=flat-square&logo=c%2B%2B&logoColor=white)
![C](https://img.shields.io/badge/C-%2300599C.svg?style=flat-square&logo=c&logoColor=white)
![Java](https://img.shields.io/badge/Java-%23ED8B00.svg?style=flat-square&logo=openjdk&logoColor=white)

**frameworks**

![React](https://img.shields.io/badge/React-%2320232a.svg?style=flat-square&logo=react&logoColor=%2361DAFB)
![NodeJS](https://img.shields.io/badge/Node.js-6DA55F?style=flat-square&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-%23404d59.svg?style=flat-square&logo=express&logoColor=%2361DAFB)
![Vue.js](https://img.shields.io/badge/Vue.js-%2335495e.svg?style=flat-square&logo=vuedotjs&logoColor=%234FC08D)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-%2338B2AC.svg?style=flat-square&logo=tailwind-css&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io-black?style=flat-square&logo=socket.io&badgeColor=010101)

**infra & data**

![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-%23DD0031.svg?style=flat-square&logo=redis&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-%23000000.svg?style=flat-square&logo=vercel&logoColor=white)
![Git](https://img.shields.io/badge/Git-%23F05033.svg?style=flat-square&logo=git&logoColor=white)

---

## stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=kunaalxoxo&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=kunaalxoxo&layout=compact&theme=tokyonight&hide_border=true" height="165"/>
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com?user=kunaalxoxo&theme=tokyonight&hide_border=true" alt="streak stats" />
</p>

---

<p align="center"><i>figuring it out one commit at a time</i></p>
