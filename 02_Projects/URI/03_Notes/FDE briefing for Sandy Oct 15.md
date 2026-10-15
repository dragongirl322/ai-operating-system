# FDE briefing for Sandy meeting (Oct 15, 2026)

## Bottom line
Forward Deployed Engineers (FDEs) take an AI product from demo to real production use inside a customer, and they're judged on adoption, not sales. The build is usually short; most time goes to pilots, evals and adoption. Public frameworks focus on use cases and model accuracy. Almost nothing public tests whether real users can do their real work with the AI and want to keep using it. That gap is URI's opening.

## What FDEs deliver
- Business: one high-value problem taken from pilot to production and used (OpenAI picks problems "worth tens of millions to billions"). Field learnings fed back to product.
- Technical: integrations, data pipelines, evals, production apps on the customer's systems.
- Sources: [LMVersity](https://lmversity.com/roles/forward-deployed-engineer/orientation/a-week-in-the-life-four-accounts), [Paluch](https://szymonpaluch.com/blog/posts/what-is-a-forward-deployed-engineer)

## Process
- Common loop: scope, build in the customer's systems, go live, measure, feed back to product.
- OpenAI (reported): Scoping (problem + one success metric), Validation (evals prove the model can hit it), Delivery. [FDE Masters](https://fdemasters.com/forward-deployed-engineer-at-palantir-openai-anthropic/)
- Palantir: Echos find the true problem, break it into workflows, align stakeholders "from the CIO to the nurse," solve backwards from the user's workflow. Deltas build. [Palantir Careers](https://www.palantir.com/careers/), [Palantir blog](https://blog.palantir.com/a-day-in-the-life-of-a-palantir-deployment-strategist-951cb59a5a96)
- Vendor playbook timeline: discovery wk 1-4, prototype by wk 6, deploy by wk 10, handoff ~day 120. [Perspective AI](https://getperspective.ai/blog/the-forward-deployed-engineer-playbook-how-to-structure-run-and-scale-an-fde-function-in-2026)

## Engagement length (as reported)
- Morgan Stanley + OpenAI: 6-8 wk build, then ~4 months of pilots and eval refinement; ~98% adoption (secondhand). [The Forward Deployed](https://www.theforwarddeployed.io/the-job)
- Range: 6-8 wk build to ~1 year embedded. Teams of 4-5. 20-50% on site.
- No public durations found for Sierra, Decagon, Harvey.

## How success is measured
- Adoption and production uptime (no sales quotas in ~1,000 FDE job ads).
- The scoping success metric and eval pass rates.
- Time to value; features shipped back to product.
- Expansion matters, but no public FDE revenue benchmarks.

## Roles and company types
- FDE / Delta: builds production code. Deployment strategist / Echo (Scale: AI Deployment Strategist): owns problem, workflow design, adoption. Solutions engineer: demos to close a sale.
- Product vendors with FDE teams: Palantir, OpenAI, Anthropic, Scale, Databricks; Sierra, Decagon, Harvey, Glean.
- SIs building FDE practices: Accenture ("largest FDE capability"; Workday FDE program announced Oct 13). [Accenture](https://newsroom.accenture.com/news/2026/accenture-launches-forward-deployed-engineering-program-with-workday-to-reinvent-work-for-the-agentic-ai-era)
- FDE-as-a-service: [Plank](https://joinplank.com/) ("build, deploy, and validate"), closest to URI's space.

## How Echo-style teams define the problem
- Palantir centers on the Ontology (map of data, actions, permissions) and "distilling functional requirements." [Palantir docs](https://palantir.com/docs/foundry/platform-overview/overview/)
- AIP Bootcamps: described only in marketing terms.
- Accenture outputs named but not public: value architecture, ROI backlogs, use case prioritization frameworks, AI adoption roadmaps.
- No real Echo artifacts are public.
- Common pattern: ranked use cases, one success metric, accuracy evals. User testing is not a named standard step.

### Artifacts you can open
- [OpenAI: Identifying and scaling AI use cases](https://openai.com/business/guides-and-resources/identifying-and-scaling-ai-use-cases/) (six use-case types, Impact/Effort grid)
- [OpenAI: A practical guide to building agents](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf) (ends "Start small, validate with real users")
- [Anthropic: Building effective agents](https://www.anthropic.com/engineering/building-effective-agents) (agent design, not customer scoping)

## How adoption is defined
- Mostly "used it at least once in the period."
- Microsoft Copilot: active users / enabled users; returning users over 7 and 28 days. [Microsoft](https://learn.microsoft.com/en-us/microsoft-365/admin/activity-reports/microsoft-365-copilot-usage?view=o365-worldwide)
- ChatGPT Enterprise: active = one message; power-user tier by volume. [OpenAI Help](https://help.openai.com/en/articles/10875114)
- GitHub Copilot: closest to outcomes; compares merged PRs and merge speed, users vs non-users. [GitHub](https://github.blog/changelog/2026-07-22-new-copilot-usage-metrics-impact-dashboard/)
- Tracking over time measures activity, not success. Share of real work handled is not standard. Palantir publishes nothing.

### Strong, then dips
- Vendor answer: more training and champions. Assumes the user is the problem; no diagnosis of the product. No public FDE playbook.

### Strong adoption, bad efficiency
- Workday: "nearly 40%" of AI time savings lost to rework; only 14% get consistently positive results. [Workday](https://newsroom.workday.com/2026-01-14-New-Workday-Research-Companies-Are-Leaving-AI-Gains-on-the-Table)
- Workslop: ~2 hours per incident, self-reported. [HBR](https://hbr.org/2026/01/why-people-create-ai-workslop-and-how-to-stop-it)
- METR: experienced devs 19% slower with AI, believed 20% faster (METR now calls this dated). [METR](https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/)
- MIT NANDA: ~95% of pilots show little P&L impact; methodology contested. [Fortune](https://fortune.com/2025/08/18/mit-report-95-percent-generative-ai-pilots-at-companies-failing-cfo/)

## Where URI fits
- Before go-live: proof real users can do their real work with the AI and want to use it.
- The pilot stretch where engagements stall.
- After launch: diagnose dips and poor efficiency, with prioritized fixes.
- For SIs promising outcomes "through adoption," an independent user verdict backs the promise.

## Questions for Sandy
1. Where do engagements stall: the build, or adoption after go-live?
2. Who owns adoption on an FDE team, and how do they gather user evidence today?
3. Has user success ever been the agreed success metric at scoping, or only model performance?
4. How is adoption defined and tracked in engagements you've seen?
5. When adoption dips, who figures out why?
6. What happens when people use it but the work is slow or needs rework?
7. Who pays for validation work, and from which budget?
8. Would an SI bring in an outside evaluator, or want to white-label it?
9. When is the best moment to bring in an evaluator like URI?
10. Which FDE firms or SIs should we talk to first?

Note: some sources are vendor blogs or secondary writeups; figures marked "reported" are secondhand.
