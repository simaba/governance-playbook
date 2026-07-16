# Enterprise AI Governance Playbook

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A practitioner playbook for designing AI governance as a decision and evidence service—not a layer of committees, generic risk tiers, and approval templates.

The repository covers the organizational system around AI work: intake, routing, prioritization, lifecycle decisions, evidence, release, monitoring, incident response, exceptions, improvement, and retirement.

## The operating-model question

A credible governance model should let an organization answer:

- Which recurring AI decisions exist?
- Who is authorized to make each one?
- Which evidence and affected-party input are required?
- How quickly must the decision be made to remain useful?
- Which path is proportional to the authority, consequence, data, and evidence maturity?
- How are conditions, exceptions, dissent, and residual risk recorded?
- Who verifies follow-through?
- Which change or incident invalidates the decision?
- How is governance burden measured and removed?

Naming an intake forum, release committee, and monitoring meeting does not answer those questions.

## Start here

| Artifact | Use it for |
|---|---|
| [`docs/operating-model-design.md`](docs/operating-model-design.md) | designing decision inventory, governance service contracts, proportional paths, forums, ownership, and metrics |
| [`templates/ai-governance-operating-model.md`](templates/ai-governance-operating-model.md) | documenting an organization-specific operating model |
| [`examples/sample-ai-governance-operating-model.md`](examples/sample-ai-governance-operating-model.md) | reviewing a fictional filled example |
| [`docs/risk-vocabulary.md`](docs/risk-vocabulary.md) | separating system risk, finding severity, control state, evaluation result, and release decision |
| [`release-governance`](https://github.com/simaba/release-governance) | detailed release-stage evidence and decision semantics |

## Design sequence

```text
scope and objectives
        ↓
recurring decision inventory
        ↓
decision rights and affected-party input
        ↓
proportional governance paths
        ↓
intake, evidence, decision, and follow-through contracts
        ↓
forums only where joint authority is needed
        ↓
metrics, cases, and operating-model improvement
```

Starting with committees usually reproduces the existing organization chart rather than designing the decisions AI systems need.

## 1. Decision inventory

List decisions across the lifecycle:

- accept, redirect, or reject a use case;
- authorize discovery, prototype, pilot, expansion, or release;
- approve data, vendor, model, tool, permission, or architecture boundaries;
- grant an exception;
- accept residual risk;
- hold, roll back, contain, or retire;
- renew an approval after material change.

For each decision, record owner, evidence, required reviewers, useful-by window, outcome vocabulary, exception path, record, and revisit trigger.

A forum with no distinct decision right is usually a status meeting.

## 2. Proportional paths

Do not let one low/medium/high label decide the entire governance route. Consider:

- consequence and reversibility;
- affected people and rights;
- data sensitivity, scale, region, and retention;
- read, write, communication, financial, code, or physical authority;
- external visibility and operational criticality;
- evidence and model maturity;
- supplier and dependency concentration;
- ability to monitor, stop, roll back, and remediate;
- legal, contractual, and policy obligations.

Possible paths include self-service validation, lightweight peer review, specialist control review, cross-functional decision, accountable-risk-owner decision, and prohibited/redesign.

Proportionality should reduce low-value review without weakening non-negotiable controls.

## 3. Governance as a service

Teams interact with governance through four contracts.

### Intake

- eligibility and exclusions;
- minimum information;
- incomplete-request handling;
- routing and response objective;
- sensitive-information boundary.

### Evidence

- propositions that must be supported;
- acceptable sources, methods, and provenance;
- freshness and invalidation;
- reviewer qualifications;
- uncertainty and disagreement;
- reuse, storage, access, and retention.

### Decision

- outcome vocabulary;
- authority and delegation;
- conditions, exceptions, and residual risk;
- turnaround objective;
- effective date, expiry, and renewal.

### Follow-through

- actions, owners, and dates;
- verification of conditions;
- escalation, incident, and stop path;
- closure evidence;
- feedback into policy, controls, tools, staffing, and training.

## 4. Forum design

For each forum, define:

- the decision it alone is authorized to make;
- eligible scope;
- decision members versus evidence and challenge members;
- pre-read and completeness requirements;
- decision outcomes;
- dissent and escalation;
- service objective;
- decision record and follow-through;
- health review and retirement criteria.

Attendance is not approval. Record who made the decision, under what authority, with which evidence and conditions.

## 5. Ownership and assurance

Keep these roles distinct where applicable:

- product or use-case owner;
- technical, data, model, tool, and platform owners;
- control owners;
- independent review or assurance;
- release and residual-risk decision owner;
- incident and remediation owner;
- redress and correction owner;
- affected-user or representative input.

Review and challenge functions should not quietly become owners of delivery controls, and product owners should not be given sole authority to accept every category of risk.

## 6. Lifecycle

| Stage | Decision emphasis |
|---|---|
| Intake | route, reject, request discovery, assign owner |
| Discovery | continue, stop, redesign, define evidence plan |
| Prototype | test feasibility and failure observability |
| Pilot | authorize bounded population, data, tools, and authority |
| Expansion / release | evaluate outcomes, controls, operations, and residual risks |
| Operation | continue, condition, adjust, pause, roll back, or renew |
| Retirement | remove access, data, memory, dependencies, and user obligations |

Each stage should define evidence, hard gates, owner, outcome, follow-through, expiry, and invalidation triggers.

## 7. Metrics that diagnose governance

Avoid treating approval rate or gate pass rate as evidence of governance quality.

Useful measures include:

### Flow and capacity

- time waiting for evidence, review, or decision authority;
- decisions made after their useful-by date;
- rework caused by unclear requirements;
- workload by route and expertise;
- duplicate reviews.

### Evidence and decision quality

- stale or missing evidence;
- reviewer disagreement and adjudication;
- decisions invalidated by untracked change;
- conditions and exceptions past expiry;
- residual risks without current owner.

### Outcomes and control

- incidents and recurrence by control path;
- stop, rollback, and remediation performance;
- user correction, complaint, appeal, or redress outcomes;
- orphaned systems, credentials, owners, and approvals;
- recurring exceptions that indicate a broken standard path.

Metrics should state their decision use and gaming risk. More reported incidents can initially indicate better detection rather than worse governance.

## 8. Improvement using real cases

Periodic review should examine decisions and incidents, not only template completion.

Ask:

- Was the decision made at the right level and in time to matter?
- Was the evidence current, relevant, and reusable?
- Which uncertainty, affected-party input, or dissent was hidden?
- Which control created false assurance or unnecessary burden?
- Which exception repeated?
- Which forum or artifact could be removed?
- What policy, staffing, tooling, or ownership change follows?

Improvement is meaningful when it changes the operating system, not only when teams receive another reminder to complete fields.

## Repository map

| Area | Content |
|---|---|
| `playbook/` | lifecycle guidance for intake, prioritization, release, monitoring, and improvement |
| `templates/` | intake, operating-model, prioritization, and review artifacts |
| `examples/` | fictional worked examples |
| `docs/` | operating-model design and risk vocabulary |
| `lean-six-sigma/` | process and measurement views for governance operations |

## Maturity and scope

This is a practitioner playbook for operating-model design. It is not a certified governance system, legal determination, compliance assessment, safety case, or official guidance from NIST, ISO, the EU, or any employer.

Adapt the decisions, evidence, authority, forums, and metrics to the actual organization, system, affected people, jurisdiction, and risk.

## Related repositories

| Repository | Distinct role |
|---|---|
| [`release-governance`](https://github.com/simaba/release-governance) | release evidence and accountable decisions |
| [`release-checklist`](https://github.com/simaba/release-checklist) | executable configuration validation |
| [`accountability-patterns`](https://github.com/simaba/accountability-patterns) | ownership, human review, provenance, explanation, and redress |
| [`nist-rmf-guide`](https://github.com/simaba/nist-rmf-guide) | practitioner navigation of NIST AI RMF |
| [`regulated-ai`](https://github.com/simaba/regulated-ai) | starter repository structure |

---

*Maintained by [Sima Bagheri](https://github.com/simaba).*
