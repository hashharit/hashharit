<div align="center">

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1f6feb,100:39d353&height=180&section=header&text=Harit%20Mohan&fontSize=52&fontColor=ffffff&animation=fadeIn&fontAlignY=35)

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1200&color=39D353&center=true&vCenter=true&width=560&lines=Backend+Engineer+%40+HealthifyMe;Ex-Amazon+SDE;I+make+LLMs+behave+in+production;Distributed+systems+%C2%B7+event-driven+backends)](https://www.linkedin.com/in/harit-mohan)

</div>

## $ whoami

```yaml
harit:
  role:      Backend Software Engineer          # SDE-1 @ HealthifyMe, ex-Amazon
  location:  Bengaluru, IN
  domain:    production LLM systems · health-tech platforms · high-scale sync
  open_to:   SDE-2 backend roles
```

Backend engineer who ships the boring-but-critical layer: the validation gates,
idempotency keys, and phased rollouts that let AI features run unsupervised in
production. Currently building LLM-powered systems serving millions of users at
HealthifyMe; previously infrastructure tooling at Amazon.

## ⚡ Tech I work with

<div align="center">

[![Skills](https://skillicons.dev/icons?i=python,django,fastapi,nodejs,ts,cpp,mysql,mongodb,kafka,graphql,redis,aws,gcp,docker,git,linux&perline=8)](https://github.com/hashharit)

</div>

## 🔧 The kind of problems I solve

- **Taming LLM output** — layered grounding pipelines that turn "plausible" model
  responses into deterministic, validated results you can serve to real users
- **Systems that sync** — loop-safe, idempotent two-way integrations between
  platforms at ~1M-user scale, over GraphQL, webhooks, and event streams
- **Migrations without incidents** — sync → async re-architecture behind parity
  suites and staged rollouts, so nobody notices anything except the speedup
- **Automation with guardrails** — replacing daily manual ops with pipelines that
  are deterministic first, LLM-assisted second, and never trusted blindly
- **Infrastructure as code** — AWS CDK pipelines that standardize how teams ship

Most of this lives in private company repos — happy to walk through the design of
any of it.

## 🧠 How I use LLMs in production

```python
result = deterministic_pipeline(input)    # always try this first
if result is None:
    result = llm_extract(input)           # extraction only — never trust generation
    result = validate_or_reject(result)   # grounded, or it doesn't ship
```

## 📈 GitHub stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=hashharit&show_icons=true&theme=github_dark&hide_border=true&count_private=true&include_all_commits=true" alt="GitHub stats" />
<img height="165" src="https://streak-stats.demolab.com?user=hashharit&theme=github-dark-blue&hide_border=true" alt="Streak" />

<img width="92%" src="https://github-readme-activity-graph.vercel.app/graph?username=hashharit&theme=github-compact&hide_border=true&area=true" alt="Activity graph" />

</div>

## 🔗 Find me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-harit--mohan-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/harit-mohan)
[![LeetCode](https://img.shields.io/badge/LeetCode-windblaze-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/windblaze)

</div>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:39d353,50:1f6feb,100:0d1117&height=100&section=footer)
