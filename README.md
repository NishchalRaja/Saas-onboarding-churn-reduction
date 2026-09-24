# Guided Onboarding & Churn Reduction - FlowStack

**Author:** Nishchal Raja | Business Analyst
**Category:** Consulting / Business Case / Process Improvement

> A self-directed portfolio project built around a simulated B2B SaaS company, "Flow Stack," to demonstrate a consulting-style engagement, from business case and strategy through requirements, delivery, and measured results.

---

## Executive Summary

FlowStack, a fictional B2B SaaS project-management tool for SMBs, was losing 22% of new paid customers within 90 days — nearly double the industry benchmark. This project built the full case for fixing it: a business case quantifying the ARR at risk, a strategy analysis weighing three options, stakeholder alignment across Customer Success, Product, and Finance, and a delivery plan that shipped guided onboarding plus a health-score alerting system for at-risk accounts — without adding CSM headcount.

---

## Business Problem

### Context
FlowStack converts trials to paid well, but new paid customers frequently churn before their first renewal. There was no structured onboarding path and no early-warning signal for accounts drifting toward churn.

### Challenge
90-day churn sat at 22% against a ~10–12% benchmark, putting an estimated $633,600 in annual ARR at risk (full breakdown in [Business_Case.md](./Business_Case.md)).

### Objective
Cut 90-day churn to 13% and lift Net Revenue Retention to 102%+, without growing the Customer Success team - full strategic reasoning in [Strategy_Analysis.md](./Strategy_Analysis.md).

---

## Methodology & Techniques Used

- **Cohort and funnel analysis**  quantified where and when new customers were stalling
- **Voice-of-customer synthesis** themed CS exit-interview notes to isolate the root cause
- **Options matrix + SWOT**  evaluated three strategic paths before recommending a hybrid approach
- **Stakeholder mapping + RACI**  aligned Customer Success, Product, Engineering, Sales, and Finance
- **Health-score modeling**  weighted usage signals (login frequency, feature adoption, checklist completion) into a daily risk score
- **Agile delivery within a phase-gated lifecycle**  waterfall-style sign-offs for strategy and requirements, two-week sprints for build (see [Project_Lifecycle.md](./Project_Lifecycle.md))
- **Pilot-then-scale rollout**  validated on 25% of new customers before full rollout

---

## Key Findings

### Finding 1: Customers had no structured path to value
**Impact:** Only ~30% of new customers reached a "first meaningful outcome" within 7 days; the rest were left to self-explore with no guidance.

### Finding 2: Churn risk was invisible until it was too late
**Impact:** No signal existed to flag a stalling account before the 90-day renewal conversation — by then, the relationship was already lost.

### Finding 3: CSM time was spread evenly, not where it mattered
**Impact:** Every account received the same light-touch attention regardless of risk, so at-risk accounts got no more help than healthy ones.

---

## Recommendations

1. **Ship an in-app guided onboarding checklist and email nudge sequence** for every new customer (Sprint 1)
2. **Build a daily health-score model** from existing usage data to flag at-risk accounts early (Sprint 2)
3. **Route only flagged accounts to CSMs** with full onboarding context, concentrating human effort where it has the most impact

Full requirements in [BRD.md](./BRD.md) and delivery-ready backlog in [User_Stories.md](./User_Stories.md).

---

## Results & Impact (Pilot)

> Simulated pilot results for this portfolio case study, modeled on the [Business_Case.md](./Business_Case.md) success criteria — not audited data from a real company.

| Metric | Before | After (Pilot, 25% of new customers) | Change |
|---|---|---|---|
| 90-day churn | 22% | 13% | **-9 points** |
| Time-to-first-value | 18 days | 6 days | **-67%** |
| Net Revenue Retention | 96% | 102% | **+6 points** |
| At-risk accounts flagged before day 60 | 0% | 84% | New capability |
| Annualized ARR retained (extrapolated) | — | ≈$410,000 | vs. $85,000 build cost |

**Bottom line:** the pilot hit its churn and time-to-value targets without adding CSM headcount, and projected ARR retention paid back the build cost in roughly 3 months.

---

## Project Files

This repository contains:

- `README.md` — This file
- `Business_Case.md` — Problem cost, options considered, financial projection, and ROI
- `Strategy_Analysis.md` — Options matrix, SWOT, and recommended strategic direction
- `Stakeholder_Analysis.md` — Stakeholder map, RACI matrix, and engagement plan
- `Project_Lifecycle.md` — Phases, timeline, and governance gates from initiation to rollout
- `BRD.md` — Business, functional, and non-functional requirements
- `User_Stories.md` — Sprint-ready backlog with acceptance criteria
- `Process_Map.md` — As-is and to-be onboarding flow diagrams

---

## Limitations & Caveats

- This is a simulated case study for portfolio purposes, not a real client engagement — figures, interviews, and pilot results are illustrative, constructed to be internally consistent rather than audited.
- The health-score model's weighting is illustrative; a real implementation would need statistical validation against actual churn outcomes.

---

## Key Learnings

1. Quantifying the cost of inaction in the business case made it far easier to get cross-functional buy-in than leading with the proposed solution.
2. A hybrid strategy — automate the scalable part, keep humans on the highest-risk part — often beats an all-or-nothing build-vs-headcount choice.
3. Phase-gating the lifecycle (sign-off at each stage) kept Finance and the executive sponsor engaged without slowing down the actual sprint-based build.

---

## Contact & Questions

**Author:** Nishchal Raja
**Email:** nishchalraja68@gmail.com
**LinkedIn:** www.linkedin.com/in/nishchal-raja

---

## License & Usage

This analysis and recommendations are provided for educational and professional portfolio purposes.
