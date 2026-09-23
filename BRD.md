# Business Requirements Document (BRD)
## Guided Onboarding & Health-Score Alerts — FlowStack

**Prepared by:** Nishchal Raja, Business Analyst
**Version:** 1.0 | **Status:** Approved for Development

---

## 1. Project Overview

FlowStack loses 22% of new paid customers within 90 days, well above the ~10–12% industry benchmark. Root cause: customers are not guided to a "first meaningful outcome" in the product before their next renewal touchpoint.

### 1.1 Business Objective
Reduce 90-day churn from 22% to 13% by combining automated in-app onboarding with a health-score model that flags at-risk accounts for proactive CSM outreach.

## 2. Scope

**In Scope**
- In-app guided onboarding checklist for all new paid customers
- Automated onboarding email nudge sequence
- Health-score model based on existing product usage data
- CRM integration to alert CSMs when an account's health score drops below threshold
- Revised CSM outreach playbook for flagged accounts

**Out of Scope**
- Pricing or packaging changes
- Enterprise-tier onboarding (already has dedicated CSM-led onboarding)
- New marketing campaigns for trial acquisition

## 3. Business Requirements

| ID | Requirement |
|---|---|
| BR-01 | Reduce 90-day churn from 22% to 13% within two quarters of full rollout |
| BR-02 | Reduce average time-to-first-value from 18 days to under 7 days |
| BR-03 | Flag at-risk accounts to CSMs with enough lead time to intervene before churn risk becomes irreversible |
| BR-04 | Achieve the above without adding CSM headcount |

## 4. Functional Requirements

| ID | Requirement |
|---|---|
| FR-01 | System shall display an in-app onboarding checklist covering the top 4 setup actions correlated with retention (invite teammate, connect an integration, create first project, complete first task) |
| FR-02 | System shall send automated email nudges for any checklist item left incomplete after 3, 7, and 14 days |
| FR-03 | System shall calculate a health score per account daily, weighted by login frequency, checklist completion, and feature adoption breadth |
| FR-04 | System shall push an alert to the CSM's CRM queue when an account's health score falls below the defined risk threshold |
| FR-05 | System shall log which onboarding actions a flagged account has and hasn't completed, visible to the CSM at the point of outreach |
| FR-06 | System shall allow Customer Success leadership to adjust the health-score threshold without an engineering change |

## 5. Non-Functional Requirements

| ID | Requirement |
|---|---|
| NFR-01 | Health-score recalculation shall complete within the nightly batch window with no customer-facing performance impact |
| NFR-02 | Onboarding checklist shall load within 1 second on the main dashboard |
| NFR-03 | Health-score model logic shall be auditable/explainable to Customer Success leadership (no black-box scoring) |

## 6. Assumptions & Constraints

- Existing product usage data (logins, feature events) is already instrumented and available
- CRM used by CSMs supports custom alert triggers via API
- No new CSM headcount will be requested as part of this initiative

## 7. Risks

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| Health-score model produces false negatives (misses at-risk accounts) | Medium | High | Manual CS review of a sample cohort during the pilot to validate model accuracy |
| CSMs over-rely on automated alerts and stop using judgment | Low | Medium | Playbook explicitly frames alerts as a supplement, not a replacement, for CS judgment |
| Onboarding checklist nudges feel like spam and get ignored | Medium | Medium | Cap nudge frequency and A/B test messaging tone during pilot |

## 8. Success Metrics / KPIs

- 90-day churn rate (target: ≤13%)
- Time-to-first-value (target: <7 days)
- Net Revenue Retention (target: 102%+)
- Health-score alert precision (validated against manual CS judgment during pilot)
