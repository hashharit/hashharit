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

<details>
<summary><b>🧵 Deep-dive: how do you make an LLM's answer <i>provably</i> correct?</b></summary>
<br>

You don't trust it — you rebuild it. The diet-plan system I designed runs every
LLM response through three grounding layers before a user ever sees it:

1. **Macro recomputation** — nutrition math is recomputed from source data, never
   taken from the model's own arithmetic
2. **Food-DB resolution** — every food item must resolve to a real database entry;
   hallucinated foods die here
3. **Algebraic serving solver** — serving sizes are solved as equations against
   the target macros, so the final plan is numerically consistent by construction

The LLM proposes; the pipeline disposes. ~900 plans/day run through this with no
human in the loop.
</details>

<details>
<summary><b>🧵 Deep-dive: shipping a rewrite with literally zero incidents</b></summary>
<br>

Moving LLM generation from Celery workers to an async FastAPI orchestrator, the
scary part isn't the new code — it's proving the new path produces identical
results. The rollout was gated by a golden-parity suite comparing old vs new
output at 1e-9 tolerance, plus shadow-running the new path on real traffic before
it served anyone. Then 5% → 25% → 60% → 100%, each stage watched. Zero incidents,
~5s faster per request.
</details>

## 🧠 How I use LLMs in production

```python
result = deterministic_pipeline(input)    # always try this first
if result is None:
    result = llm_extract(input)           # extraction only — never trust generation
    result = validate_or_reject(result)   # grounded, or it doesn't ship
```

## 📦 Things I've built in the open

Most of my production work lives in private company repos — these are side projects:

<div align="center">

[![CP-Progress-Tracker](https://github-readme-stats.vercel.app/api/pin/?username=hashharit&repo=CP-Progress-Tracker&theme=github_dark&hide_border=true)](https://github.com/hashharit/CP-Progress-Tracker)
[![Google-Scraper](https://github-readme-stats.vercel.app/api/pin/?username=hashharit&repo=Google-Scraper&theme=github_dark&hide_border=true)](https://github.com/hashharit/Google-Scraper)
[![hide-text](https://github-readme-stats.vercel.app/api/pin/?username=hashharit&repo=hide-text&theme=github_dark&hide_border=true)](https://github.com/hashharit/hide-text)
[![affiliate-link-batch](https://github-readme-stats.vercel.app/api/pin/?username=hashharit&repo=affiliate-link-batch&theme=github_dark&hide_border=true)](https://github.com/hashharit/affiliate-link-batch)

</div>

## 📈 Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=hashharit&show_icons=true&theme=github_dark&hide_border=true&count_private=true&include_all_commits=true" alt="GitHub stats" />
<img height="165" src="https://streak-stats.demolab.com?user=hashharit&theme=github-dark-blue&hide_border=true" alt="Streak" />

<a href="https://leetcode.com/windblaze"><img width="460" src="https://leetcard.jacoblin.cool/windblaze?theme=dark&font=Fira%20Code&ext=heatmap" alt="LeetCode stats" /></a>

<img width="92%" src="https://github-readme-activity-graph.vercel.app/graph?username=hashharit&theme=github-compact&hide_border=true&area=true" alt="Activity graph" />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/hashharit/hashharit/output/github-snake.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/hashharit/hashharit/output/github-snake-light.svg" />
  <img alt="contribution snake" src="https://raw.githubusercontent.com/hashharit/hashharit/output/github-snake-light.svg" />
</picture>

</div>

## 🔗 Find me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-harit--mohan-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/harit-mohan)
[![LeetCode](https://img.shields.io/badge/LeetCode-windblaze-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/windblaze)

</div>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:39d353,50:1f6feb,100:0d1117&height=100&section=footer)
