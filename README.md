<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=26&pause=1000&color=6C63FF&center=true&vCenter=true&width=700&lines=Hey%2C+I'm+Kunaal+Lala+%F0%9F%91%8B;AI+Engineer+%7C+Open-Source+Builder;Making+NVIDIA+engineers+nervous+since+2025;GSoC+2026+Applicant+%7C+BITS+Pilani+Hyderabad" alt="Typing SVG" />
</div>

<p align="center">
  <b>2nd-year undergrad @ BITS Pilani Hyderabad</b> &middot; Building LLM-powered tools, automating everything in sight, and making GPU code portable one <code>.cu</code> file at a time.
</p>

<p align="center">
  <a href="https://linkedin.com/in/kunaal-lala"><img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://instagram.com/kunaalxoxo"><img src="https://img.shields.io/badge/Instagram-%23E4405F.svg?style=for-the-badge&logo=Instagram&logoColor=white"/></a>
  <a href="https://reddit.com/user/-bhAAi-"><img src="https://img.shields.io/badge/Reddit-%23FF4500.svg?style=for-the-badge&logo=Reddit&logoColor=white"/></a>
  <a href="mailto:urfav.kunaal@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
</p>

---

## 🚀 Featured: cuda-migrator

> *CUDA lock-in is just NVIDIA's way of saying "please don't leave us." I built a tool that says bye.*

**[cuda-migrator](https://github.com/kunaalxoxo/cuda-migrator)** is an LLM-powered tool that automatically migrates CUDA (`.cu`) code to AMD ROCm/HIP — making GPU code portable across NVIDIA and AMD hardware in **12 seconds** instead of **2–4 weeks**.

```
.cu → AST Parse → 65 Deterministic Rules → hipcc Validate → MI300X Benchmark → Report
```

- 🔍 **Zero regex** — tree-sitter AST analysis, not grep-and-pray
- ⚡ **65 deterministic transformation rules** across 7 categories (headers, memory API, streams, events, enums...)
- 🤖 **LLM fallback** via DeepSeek R1 on OpenRouter — only for edge cases, always compile-validated. Hallucinations get rejected automatically.
- 📊 **Dual-format reporting** — JSON + Rich terminal panels for every migration run
- ☁️ **3 compile modes**: stub (no AMD hardware needed), local hipcc, AMD Developer Cloud MI300X

| Kernel | Status | Rules Fired | Throughput Delta |
|--------|--------|-------------|-----------------|
| `softmax.cu` | ✅ PASS | 21 | +3.2% on MI300X |
| `gemm.cu` | ✅ PASS | 15 | +1.8% on MI300X |
| `attention.cu` | ⚠️ WARN (intentional) | 19 | +2.1% on MI300X |

> AMD MI300X is 30–40% cheaper per FLOP than NVIDIA H100. The only thing stopping enterprises from switching? 3 million production CUDA kernels. This tool fixes that.

**[→ View Repository](https://github.com/kunaalxoxo/cuda-migrator)** &middot; **[→ pip install cuda-migrator](https://github.com/kunaalxoxo/cuda-migrator#installation)**

---

## 🧠 What I Do

```python
kunaal = {
    "role":     ["AI/ML Engineer", "CRM Developer", "Open-Source Builder"],
    "building": "tools that solve real problems (and yes, also a todo app — it deploys though)",
    "skills":   {
        "AI/ML":      ["LLM tooling", "Python", "NumPy", "Pandas", "scikit-learn"],
        "CRM":        ["Zoho CRM", "Deluge scripting", "workflow automation"],
        "Full-Stack": ["React", "Node.js", "Vue.js", "TailwindCSS"],
        "DevOps":     ["Docker", "Vercel", "Netlify", "Render"],
    },
    "currently_chasing": ["GSoC 2026", "Microsoft Explore", "Claude for OSS 🤞"],
    "fun_fact": "built cuda-migrator in one sitting. the commit timestamps are evidence.",
}
```

---

## 🎯 Current Focus

- 🛠️ Growing **[cuda-migrator](https://github.com/kunaalxoxo/cuda-migrator)** — Phase 2 (real hipcc + rocprof benchmarking) is next. Contributions welcome
- 🔍 Applying for **Microsoft Explore Program** and **GSoC 2026**
- 📊 Building a data science portfolio with Python, pandas, and scikit-learn
- ☕ Running on chai and questionable sleep schedules

---

## 🌐 Other Projects

| Project | Description | Live |
|---------|-------------|------|
| Todo List App | Full-stack task manager (everyone builds one, mine actually works) | [🔗](https://todo-list-app-zj31.onrender.com) |
| News Aggregator | Real-time news feed — because doom-scrolling deserves some structure | [🔗](https://news-aggregator-4mvu.onrender.com) |
| Notes App | Clean markdown notes app | [🔗](https://dynamic-kelpie-90b880.netlify.app/) |

---

## 💻 Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3670A0?style=flat-square&logo=python&logoColor=ffdd54)
![JavaScript](https://img.shields.io/badge/JavaScript-%23323330.svg?style=flat-square&logo=javascript&logoColor=%23F7DF1E)
![C++](https://img.shields.io/badge/C++-%2300599C.svg?style=flat-square&logo=c%2B%2B&logoColor=white)
![C](https://img.shields.io/badge/C-%2300599C.svg?style=flat-square&logo=c&logoColor=white)
![Java](https://img.shields.io/badge/Java-%23ED8B00.svg?style=flat-square&logo=openjdk&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-%23E34F26.svg?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-%231572B6.svg?style=flat-square&logo=css3&logoColor=white)

**Frameworks & Libraries**

![React](https://img.shields.io/badge/React-%2320232a.svg?style=flat-square&logo=react&logoColor=%2361DAFB)
![NodeJS](https://img.shields.io/badge/Node.js-6DA55F?style=flat-square&logo=node.js&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js-%2335495e.svg?style=flat-square&logo=vuedotjs&logoColor=%234FC08D)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-%2338B2AC.svg?style=flat-square&logo=tailwind-css&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-%23013243.svg?style=flat-square&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-%23150458.svg?style=flat-square&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=flat-square&logo=scikit-learn&logoColor=white)

**Databases & Cloud**

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=flat-square&logo=mongodb&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-%23000000.svg?style=flat-square&logo=vercel&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-%23000000.svg?style=flat-square&logo=netlify&logoColor=white)

**Tools**

![Git](https://img.shields.io/badge/Git-%23F05033.svg?style=flat-square&logo=git&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-%23F24E1E.svg?style=flat-square&logo=figma&logoColor=white)
![Jira](https://img.shields.io/badge/Jira-%230A0FFF.svg?style=flat-square&logo=jira&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-%23000000.svg?style=flat-square&logo=notion&logoColor=white)

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=kunaalxoxo&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=kunaalxoxo&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&layout=compact" height="165"/>
</p>

<p align="center">
  <img src="https://nirzak-streak-stats.vercel.app/?user=kunaalxoxo&theme=tokyonight&hide_border=true"/>
</p>
