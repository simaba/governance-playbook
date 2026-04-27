# AI Governance Operating Model

Use this template to define how an organization governs AI from idea intake through release, monitoring, and continuous improvement.

## 1. Operating Model Summary

| Field | Value |
|---|---|
| Organization / team | `[TBD]` |
| Scope | `[enterprise / business unit / product line / platform]` |
| Effective date | `[TBD]` |
| Owner | `[TBD]` |
| Review cadence | `[monthly / quarterly / biannual]` |
| Primary frameworks referenced | `[NIST AI RMF / ISO 42001 / EU AI Act / internal policy]` |

## 2. Governance Principles

Define the principles that guide AI decisions.

- **Accountability:** `[who owns system outcomes]`
- **Traceability:** `[what evidence must be retained]`
- **Risk proportionality:** `[how controls scale by risk tier]`
- **Human oversight:** `[where human review is mandatory]`
- **Continuous improvement:** `[how post-release learning feeds back into governance]`

## 3. Scope of AI Systems

### In scope

- `[TBD]`

### Out of scope

- `[TBD]`

### System inventory expectations

Every AI system should have:

- named business owner
- named technical owner
- use-case description
- risk tier
- release status
- model or vendor dependency
- monitoring owner
- review date

## 4. Governance Forums and Decision Rights

| Forum / role | Decision rights | Inputs required | Outputs |
|---|---|---|---|
| AI Intake Forum | `[accept / reject / request more info]` | intake form, use case summary | triage decision |
| Prioritization Forum | `[rank / defer / escalate]` | impact score, risk score, effort estimate | prioritized portfolio |
| Release Gate Review | `[approve / conditional / hold / reject]` | validation evidence, risk assessment, release plan | release decision |
| Monitoring Review | `[continue / adjust / rollback / retire]` | production metrics, incidents, drift reports | improvement actions |

## 5. Lifecycle Controls

| Stage | Minimum controls | Required artifacts |
|---|---|---|
| Intake | use-case definition, ownership, preliminary risk screen | intake form |
| Prioritization | value, risk, feasibility, dependency scoring | prioritization matrix |
| Delivery governance | milestone reviews, risk tracking, data governance | project RAID, model card draft |
| Release readiness | validation, legal/compliance review, monitoring readiness | release gate review, checklist report |
| Post-release monitoring | performance, drift, incidents, user feedback | monitoring dashboard, incident log |
| Improvement / retirement | periodic review, remediation, decommissioning decision | improvement review or retirement note |

## 6. Risk Tiering

| Tier | Definition | Example controls |
|---|---|---|
| Low | limited impact, internal use, reversible | technical review, basic monitoring |
| Medium | customer-facing or operationally significant | governance review, model card, rollback plan |
| High | regulated, safety-adjacent, hard to reverse, or high-impact | legal/compliance review, human oversight, red-team testing, formal sign-off |

## 7. Metrics and CTQs

Define governance health metrics.

| Metric | Purpose | Owner | Review cadence |
|---|---|---|---|
| AI system inventory completeness | confirms traceability | `[TBD]` | `[TBD]` |
| release gate pass rate | tracks release quality | `[TBD]` | `[TBD]` |
| incident recurrence rate | tracks control effectiveness | `[TBD]` | `[TBD]` |
| open high-risk actions | tracks unresolved exposure | `[TBD]` | `[TBD]` |
| time from intake to decision | tracks governance flow efficiency | `[TBD]` | `[TBD]` |

## 8. Escalation Rules

Escalate when:

- high-risk system lacks named owner
- required release evidence is missing
- incident severity exceeds threshold
- model behavior materially deviates from validated behavior
- legal, privacy, or safety concerns are unresolved

## 9. Continuous Improvement Loop

At each review cycle, capture:

- what failed or slowed down
- what evidence was missing
- which controls were too weak or too heavy
- what should be standardized
- which templates, checklists, or approval rules need updates

## 10. Open Decisions

| Decision | Owner | Due date | Status |
|---|---|---|---|
| `[TBD]` | `[TBD]` | `[TBD]` | `[open / decided]` |
