# Process Map — Guided Onboarding & Health-Score Alerts

## As-Is Process (Current State)

```mermaid
flowchart TD
    A[Customer converts trial to paid] --> B[Account provisioned]
    B --> C[Customer self-explores product - no guidance]
    C --> D{Customer finds value on their own?}
    D -- Yes --> E[Customer becomes engaged, likely to renew]
    D -- No --> F[Customer stalls, no one notices]
    F --> G[90-day mark reached]
    G --> H{Renewal conversation}
    H -- Too late --> I[Customer churns]
```

**Pain points identified**
- No structured guidance after signup — success depends entirely on the customer's own initiative
- No mechanism exists to detect a stalled account before the renewal conversation
- By the time churn risk is visible, it's usually too late to intervene

## To-Be Process (Redesigned)

```mermaid
flowchart TD
    A[Customer converts trial to paid] --> B[Account provisioned]
    B --> C[In-app onboarding checklist shown]
    C --> D[Automated email nudges for incomplete steps]
    D --> E[Daily health score calculated from usage data]
    E --> F{Health score below threshold?}
    F -- No --> G[Customer proceeds toward renewal, tracked passively]
    F -- Yes --> H[CSM alerted with onboarding context]
    H --> I[CSM proactive outreach]
    I --> J[Customer re-engages or churn risk resolved early]
```

**Key changes**
- Guidance is built into the product from day one instead of left to chance
- A daily health score replaces "no signal until renewal" with an early-warning system
- CSM effort is concentrated only on flagged, at-risk accounts — not spread evenly across every account

## Estimated Funnel Impact

| Stage | As-Is | To-Be Target |
|---|---|---|
| Reaches first meaningful outcome within 7 days | ~30% | 70%+ |
| At-risk accounts identified before day 60 | 0% (no signal) | 80%+ |
| 90-day churn | 22% | 13% |
