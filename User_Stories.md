# User Stories — Guided Onboarding & Health-Score Alerts

Derived from the [BRD](./BRD.md) functional requirements (FR-01 through FR-06), organized into three epics.

---

## Epic 1: In-App Guided Onboarding
*Related requirements: FR-01, FR-02*

### US-01 — Onboarding checklist
**As a** new customer, **I want** to see a short checklist of key setup steps, **so that** I know exactly what to do to get value from the product quickly.

**Acceptance Criteria**
- Given a new account's first login, when the dashboard loads, then a checklist of 4 items appears (invite teammate, connect integration, create first project, complete first task).
- Given a checklist item is completed, when the action is detected, then it's marked complete in real time.

**Priority:** Must Have | **Story Points:** 5

### US-02 — Onboarding email nudges
**As a** new customer who hasn't finished setup, **I want** a reminder email about what's left, **so that** I don't forget to finish onboarding.

**Acceptance Criteria**
- Given a checklist item is incomplete after 3, 7, or 14 days, when the nudge job runs, then an email is sent listing only the remaining items.
- Given all checklist items are complete, when the nudge job runs, then no further emails are sent.

**Priority:** Must Have | **Story Points:** 3

---

## Epic 2: Health-Score Model
*Related requirements: FR-03, FR-06*

### US-03 — Daily health score calculation
**As a** Customer Success leader, **I want** every account scored daily on retention risk, **so that** at-risk accounts can be identified before renewal.

**Acceptance Criteria**
- Given usage data for an account, when the nightly job runs, then a health score is calculated from login frequency, checklist completion, and feature-adoption breadth.
- Given an account's score is calculated, when the calculation completes, then the score and its contributing factors are stored and visible to CS ops.

**Priority:** Must Have | **Story Points:** 8

### US-04 — Adjustable risk threshold
**As a** Head of Customer Success, **I want** to adjust the health-score alert threshold, **so that** I can tune alert volume without waiting on engineering.

**Acceptance Criteria**
- Given a threshold-setting screen, when a new value is saved, then it takes effect on the next scoring run without a code deployment.

**Priority:** Should Have | **Story Points:** 3

---

## Epic 3: CSM Alerting & Outreach
*Related requirements: FR-04, FR-05*

### US-05 — CRM alert for at-risk accounts
**As a** CSM, **I want** to be alerted when one of my accounts becomes at-risk, **so that** I can reach out before they churn.

**Acceptance Criteria**
- Given an account's health score falls below threshold, when the daily scoring job completes, then an alert appears in the CSM's CRM queue.
- Given multiple accounts drop below threshold on the same day, when alerts are generated, then each is a separate, individually actionable item.

**Priority:** Must Have | **Story Points:** 5

### US-06 — Onboarding context at point of outreach
**As a** CSM reaching out to an at-risk account, **I want** to see which onboarding steps they have and haven't completed, **so that** my outreach is specific and useful rather than generic.

**Acceptance Criteria**
- Given a CSM opens an alerted account, when the account detail view loads, then completed and incomplete checklist items are both visible.

**Priority:** Must Have | **Story Points:** 3

---

## Sprint Planning Summary

**Total estimated story points:** 27

| Sprint | Stories | Points |
|---|---|---|
| Sprint 1 | US-01, US-02, US-05 | 13 |
| Sprint 2 | US-03, US-04, US-06 | 14 |
