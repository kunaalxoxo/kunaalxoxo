<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&pause=1000&color=F97316&center=true&vCenter=true&width=700&lines=hey%2C+i'm+kunaal+👋;19+from+vijayawada%2C+building+in+kochi;i+ship+things+that+actually+run;vibe+coder+%7C+systems+builder+%7C+gsc+2026" alt="Typing SVG" />
</div>

<p align="center">
  2nd-year @ BITS Pilani Hyderabad &middot; Vijayawada → Hyderabad → Kochi &middot; building things that solve real problems, not just pass interviews
</p>

<p align="center">
  <a href="https://linkedin.com/in/kunaal-lala"><img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:urfav.kunaal@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://instagram.com/kunaalxoxo"><img src="https://img.shields.io/badge/Instagram-%23E4405F.svg?style=for-the-badge&logo=instagram&logoColor=white"/></a>
</p>

---

i grew up in vijayawada, moved to hyderabad for college, and right now i'm working out of kochi. no big network, no alumni connections handing me opportunities. just me, a laptop, and a tendency to stay up too late fixing things that almost work.

most of what i build is around automation and systems — the kind of stuff where there's a messy manual process and i want to know if i can make it disappear. sometimes i build GPU tooling. sometimes i build HR pipelines. depends on what's broken.

---

## the main thing: cuda-migrator

> *CUDA lock-in is just NVIDIA's way of saying "please don't leave." this tool says bye.*

**[cuda-migrator](https://github.com/kunaalxoxo/cuda-migrator)** migrates `.cu` CUDA code to AMD ROCm/HIP automatically — what used to take 2–4 weeks now takes about 12 seconds.

```
.cu → AST parse → 65 deterministic rules → hipcc validate → MI300X benchmark → report
```

- no regex. tree-sitter AST analysis, because grep-and-pray isn't a migration strategy
- 65 transformation rules across headers, memory API, streams, events, enums
- LLM fallback via DeepSeek R1 (OpenRouter) — only for edge cases, compile-validated. hallucinations get auto-rejected
- runs in 3 modes: stub (no AMD hardware), local hipcc, AMD Developer Cloud MI300X

| kernel | status | rules fired | throughput delta |
|--------|--------|-------------|-----------------|
| softmax.cu | ✅ pass | 21 | +3.2% on MI300X |
| gemm.cu | ✅ pass | 15 | +1.8% on MI300X |
| attention.cu | ⚠️ warn (intentional) | 19 | +2.1% on MI300X |

AMD MI300X is 30–40% cheaper per FLOP than H100. the only thing stopping enterprises from switching is ~3 million production CUDA kernels. that's the problem this solves.

**[→ repo](https://github.com/kunaalxoxo/cuda-migrator)**

---

## and platepulse

**[platepulse](https://github.com/kunaalxoxo/platepulse)** — because food tracking apps either look clinical or require a nutrition degree to use. built this to actually enjoy logging meals, not dread it.

full-stack, real data, ships and runs. that's the standard i hold everything to.

---

## what i actually know

```python
kunaal = {
    "currently":  "kochi, kerala — working & building",
    "base":       "bits pilani hyderabad",
    "hometown":   "vijayawada, andhra pradesh",
    "ai_ml":      ["LLM tooling", "python", "numpy", "pandas", "scikit-learn"],
    "systems":    ["CUDA → ROCm migration", "tree-sitter AST", "GPU benchmarking"],
    "crm":        ["zoho CRM", "zoho people", "deluge scripting", "workflow automation"],
    "fullstack":  ["react", "node.js", "vue.js", "tailwind"],
    "devops":     ["docker", "vercel", "netlify", "render"],
    "chasing":    ["GSoC 2026", "VibeCon India", "building something people actually use"],
    "fun_fact":   "built cuda-migrator in one sitting. the commit timestamps are evidence.",
}
```

---

## other stuff that runs

| project | what it is | link |
|---------|-----------|------|
| platepulse | food tracking that doesn't feel like homework | [→](https://github.com/kunaalxoxo/platepulse) |
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
![Vue.js](https://img.shields.io/badge/Vue.js-%2335495e.svg?style=flat-square&logo=vuedotjs&logoColor=%234FC08D)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-%2338B2AC.svg?style=flat-square&logo=tailwind-css&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-%23013243.svg?style=flat-square&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-%23150458.svg?style=flat-square&logo=pandas&logoColor=white)

**infra**

![Docker](https://img.shields.io/badge/Docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=flat-square&logo=mongodb&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-%23000000.svg?style=flat-square&logo=vercel&logoColor=white)
![Git](https://img.shields.io/badge/Git-%23F05033.svg?style=flat-square&logo=git&logoColor=white)

---

## stats

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=kunaalxoxo&theme=tokyonight" height="165"/>
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=kunaalxoxo&theme=tokyonight" height="165"/>
</p>

<p align="center">
  <img src="https://nirzak-streak-stats.vercel.app/?user=kunaalxoxo&theme=tokyonight&hide_border=true"/>
</p>

---

<p align="center">
  <i>vijayawada kid figuring it out one commit at a time</i>
</p>
