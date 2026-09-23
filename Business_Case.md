# Business Case
## Reducing Early Churn Through Guided Onboarding — FlowStack

**Prepared by:** Nishchal Raja, Business Analyst
**Company (simulated):** FlowStack — a fictional B2B SaaS project-management tool for SMBs, used as the scenario for this case study

---

## 1. Problem Statement

FlowStack converts trials to paid subscriptions well, but **22% of new paid customers churn within their first 90 days** — nearly double the ~10–12% benchmark for SaaS tools at a similar price point ($4,800 average annual contract value). Exit surveys and CS notes point to the same root cause: customers self-serve their way into the product, never reach a "first meaningful outcome," and lapse before renewal conversations even happen.

## 2. Cost of Inaction

- ~600 new paid customers close per quarter
- At 22% 90-day churn, that's **~132 lost customers per quarter**
- At $4,800 ACV, that's **≈$633,600 in ARR at risk annually** if the pattern continues unaddressed
- Beyond direct ARR loss: CAC on churned accounts is unrecovered, and early churn suppresses expansion revenue that would otherwise come from accounts that stick past 90 days

## 3. Options Considered

| Option | Description | Cost | Speed to Value | Scalability |
|---|---|---|---|---|
| **A — Scale CSM headcount** | Hire additional Customer Success Managers to manually guide every new account | High (ongoing headcount cost) | Slow (hiring + ramp time) | Poor — cost scales linearly with customer growth |
| **B — Fully self-serve product-led onboarding** | Build in-app guided setup and automated email nudges; no human touch | Medium (one-time build) | Fast to build, slower to prove | Excellent — scales with zero marginal cost |
| **C — Hybrid: guided in-app onboarding + health-score-triggered CSM outreach** | Automated onboarding for all customers, with a health-score model flagging at-risk accounts for a human check-in | Medium (one-time build + light CSM process change) | Fast | Good — CSM effort concentrated only where it's needed |

## 4. Recommendation

**Option C (Hybrid)** is recommended. It captures most of the scalability of a pure product-led approach while preserving a human safety net for the accounts most likely to churn — avoiding both the cost of Option A and the risk of Option B leaving struggling customers with no path to help. Full rationale in [Strategy_Analysis.md](./Strategy_Analysis.md).

## 5. Financial Projection

| Item | Estimate |
|---|---|
| Build cost (design + engineering, ~2 sprints, plus PM time) | ≈$85,000 one-time |
| CSM process change (no new headcount, revised playbook) | ≈$0 incremental |
| Target 90-day churn after launch | 13% (vs. 22% baseline) |
| Projected annual ARR retained | ≈$410,000 |
| Payback period | ≈3 months of retained ARR |

## 6. Success Criteria

- 90-day churn reduced from 22% to 13% or lower within two quarters of full rollout
- Net Revenue Retention (NRR) improves from 96% to 102%+
- Time-to-first-value (first key in-product action) drops from an 18-day average to under 7 days

Actual pilot results are documented in the [README](./README.md#-results--impact-pilot).
