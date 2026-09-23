# Project Lifecycle
## Onboarding Strategy — FlowStack

A hybrid waterfall-to-agile lifecycle: strategy and requirements were sequenced up front (given cross-team budget and sign-off needs), while build and rollout ran in two-week agile sprints.

---

## Phase 1: Initiation (Weeks 1–2)
- Problem validated using churn cohort data and CS exit-interview themes
- Business case drafted and approved by COO (see [Business_Case.md](./Business_Case.md))
- Project sponsor and core working team confirmed

## Phase 2: Strategy & Planning (Weeks 3–4)
- Options analysis and SWOT completed; hybrid strategy selected (see [Strategy_Analysis.md](./Strategy_Analysis.md))
- Stakeholder map and RACI finalized (see [Stakeholder_Analysis.md](./Stakeholder_Analysis.md))
- BRD drafted and signed off by Product and Customer Success (see [BRD.md](./BRD.md))

## Phase 3: Design (Weeks 5–6)
- In-app onboarding flow wireframed
- Health-score model variables defined (usage signals: login frequency, key-feature adoption, invite-teammate action, integration setup)
- User stories written and estimated (see [User_Stories.md](./User_Stories.md))
- As-is / to-be onboarding process mapped (see [Process_Map.md](./Process_Map.md))

## Phase 4: Build (Weeks 7–10, 2 sprints)
- Sprint 1: Automated in-app onboarding checklist and email nudge sequence
- Sprint 2: Health-score model + CSM alert integration into existing CRM

## Phase 5: Pilot (Weeks 11–14)
- Rolled out to 25% of new paid customers (randomized)
- CSMs trained on the revised, health-score-triggered outreach playbook
- Weekly review of pilot cohort churn and health-score accuracy against manual CS judgment

## Phase 6: Rollout & Monitoring (Weeks 15+)
- Expanded to 100% of new paid customers after pilot go/no-go review
- 90-day churn and NRR tracked against the [Business_Case.md](./Business_Case.md) success criteria
- Quarterly review cadence established with Finance and the COO

---

## Governance & Phase Gates

| Gate | Decision | Owner |
|---|---|---|
| End of Initiation | Approve business case | COO |
| End of Planning | Approve strategy & requirements | Head of CS, VP Product |
| End of Design | Approve scope for build | Working team |
| End of Pilot | Go / no-go for full rollout | COO, Head of CS, VP Product |
