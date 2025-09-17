# Codoki AI Benchmarks (2025)

This repository serves as the **index for Codoki's reproducible AI code-review benchmarks**.  
We recreated real-world bugs across multiple open-source projects, opened fresh PRs, and measured how Codoki and other tools perform in catching them.

---

## Methodology

**Dataset.**  
50 real bugs across **Sentry (Python)**, **Grafana (Go)**, **Cal.com (TypeScript)**, **Keycloak (Java)**, and **Discourse (Ruby)**.  
Each bug maps to an upstream PR that fixed a production defect.

**Procedure.**  
We recreated the original bug PRs and ran **Codoki** on the same diffs and repository context.  
A bug counted as “caught” only when Codoki identified the fault in a **line-level PR comment** with actionable guidance.  
Mentions only in summaries did not count.

> **Competitor scores:** Results for Greptile, Cursor, GitHub Copilot, CodeRabbit, and Graphite  
> are reproduced from [Greptile’s public benchmark dataset](https://github.com/orgs/ai-code-review-evaluation/repositories).  
> We did not re-run competitor tools. Accessed: **Sept 2025**.

---

## Dataset Index

| Repository  | Language   | Dataset / Recreated PRs |
|-------------|-----------|------------------------|
| **Sentry**    | Python     | [sentry-codoki](https://github.com/codoki-ai/sentry-codoki) |
| **Cal.com**   | TypeScript | [calcom-codoki](https://github.com/codoki-ai/cal.com-codoki) |
| **Grafana**   | Go         | [grafana-codoki](https://github.com/codoki-ai/grafana-codoki) |
| **Keycloak**  | Java       | [keycloak-codoki](https://github.com/codoki-ai/keycloak-codoki) |
| **Discourse** | Ruby       | [discourse-codoki](https://github.com/codoki-ai/discourse-codoki) |

---

## Why This Matters

Engineering leaders need **transparent, reproducible benchmarks** to make informed adoption decisions.  
This dataset helps teams compare tools on realistic production bugs — not trivial synthetic demos.

---

## Contributing

- Found a bug we should add to the dataset? Open an issue or PR.
- Want to replicate this benchmark with your own tool? Fork this repo and run the same PR set.

---

## Related Links

- 📊 **Greptile Public Dataset:** [ai-code-review-evaluation](https://github.com/orgs/ai-code-review-evaluation/repositories)
- 🧪 **Codoki Website:** [codoki.ai](https://codoki.ai)

---

_Last updated: September 2025_
