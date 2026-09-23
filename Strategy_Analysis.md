# Strategy Analysis
## Onboarding Strategy — FlowStack

---

## 1. Strategic Context

FlowStack's broader company strategy for the year is "efficient growth" — improving unit economics (CAC payback, NRR) rather than growing headcount in step with new-logo growth. Any onboarding fix needs to work within that constraint: it can't rely on indefinitely scaling the CS team.

## 2. Options Matrix

| Criteria | A: Scale CSM Headcount | B: Fully Self-Serve | C: Hybrid (Recommended) |
|---|---|---|---|
| Cost | High, recurring | Medium, one-time | Medium, one-time |
| Speed to value | Slow (hiring cycle) | Fast to build | Fast to build |
| Scalability | Poor | Excellent | Good |
| Risk | Budget risk if growth accelerates | At-risk accounts may fall through with no human touch | Requires an accurate health-score model to target CSM effort well |
| Fit with "efficient growth" strategy | Poor — adds fixed cost | Good | Good |

## 3. SWOT of Current Onboarding Approach

**Strengths**
- Product is genuinely easy to set up for technically confident users
- Existing CS team has strong relationships with enterprise-tier accounts

**Weaknesses**
- No structured onboarding path for self-serve/SMB accounts
- No early-warning signal for accounts drifting toward churn
- CSM time is spread evenly across all accounts regardless of risk

**Opportunities**
- In-app usage data already exists and is unused for churn prediction
- A lightweight health-score model could redirect existing CSM capacity to where it matters most, with no new hires

**Threats**
- Competitors in the SMB project-management space have invested heavily in self-serve onboarding UX
- Continued 22% churn compounds — each lost cohort reduces the installed base that expansion revenue could come from

## 4. Recommended Strategic Direction

Adopt a **product-led onboarding motion with a human-assisted safety net**: automate the onboarding path for every new customer, and build a health-score model from existing usage data to flag accounts that aren't progressing — routing only those accounts to a CSM for a proactive check-in. This aligns with the efficient-growth mandate (no new headcount) while directly targeting the root cause (customers stalling out before reaching value) rather than only treating churn after it happens.

## 5. Key Trade-offs Accepted

- Slower initial rollout than a "hire more CSMs" fix, in exchange for a solution that scales with the business
- Dependency on health-score model accuracy — a false-negative risk is accepted and mitigated with a manual review step during the pilot (see [Project_Lifecycle.md](./Project_Lifecycle.md))
