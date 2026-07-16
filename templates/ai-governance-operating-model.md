# AI Governance Operating Model Template

Use this template to define how the organization makes, records, executes, and revisits AI-related decisions. Do not begin by naming committees. Begin with recurring decisions, evidence, authority, and follow-through.

## 1. Purpose and scope

| Field | Definition |
|---|---|
| Organization / unit | `[TBD]` |
| Systems and lifecycle stages in scope | `[TBD]` |
| Explicit exclusions | `[TBD]` |
| Operating-model owner | `[TBD]` |
| Effective date | `[TBD]` |
| Next design review | `[TBD]` |
| Authoritative policies and sources | `[TBD]` |

### Objectives

- Which decisions should become more timely, consistent, or accountable?
- Which harms, control failures, or operating burdens should the model reduce?
- Which responsibilities remain outside this operating model?

## 2. Decision inventory

| Decision ID | Decision | Lifecycle stage | Accountable owner | Required reviewers / affected input | Useful-by window | Record | Revisit trigger |
|---|---|---|---|---|---|---|---|
| DEC-001 | accept, redirect, or reject a use case | intake | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | scope or risk changes |
| DEC-002 | authorize bounded pilot | pre-pilot | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | tool, data, population, or evidence changes |
| DEC-003 | expand, hold, roll back, or retire | operation | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | incident, drift, control, or value trigger |

For every decision, define the standard outcome vocabulary: approve, approve with conditions, hold, reject, defer, escalate, retire, or another controlled set.

## 3. Proportional governance paths

Define routing dimensions rather than relying only on one low/medium/high score.

| Dimension | Questions | Routing consequence |
|---|---|---|
| Consequence and reversibility | What is the worst credible effect and can it be reversed? | `[TBD]` |
| People and rights | Who is affected, including non-users? | `[TBD]` |
| Data | sensitivity, scale, provenance, region, retention | `[TBD]` |
| Authority | read, draft, write, publish, decide, physical / financial action | `[TBD]` |
| Externality | internal, public, legal, safety, financial, infrastructure | `[TBD]` |
| Evidence maturity | exploratory, tested, validated, operationally observed | `[TBD]` |
| Control and recovery | monitor, stop, roll back, remediate | `[TBD]` |
| Obligations | legal, contractual, sector, internal policy | `[TBD]` |

### Paths

| Path | Eligibility | Review and evidence | Decision authority | Typical expiry |
|---|---|---|---|---|
| Self-service | `[TBD]` | automated validation + owner attestation | `[TBD]` | `[TBD]` |
| Lightweight review | `[TBD]` | peer or control-owner review | `[TBD]` | `[TBD]` |
| Specialist review | `[TBD]` | named domain / security / privacy / safety review | `[TBD]` | `[TBD]` |
| Cross-functional decision | `[TBD]` | integrated evidence package | `[TBD]` | `[TBD]` |
| Executive / risk acceptance | `[TBD]` | residual-risk and alternatives record | `[TBD]` | `[TBD]` |
| Prohibited / redesign | `[TBD]` | rationale and permitted alternative | `[TBD]` | until policy change |

## 4. Governance service contract

### Intake

- eligible requests:
- minimum information:
- incomplete-request handling:
- routing owner:
- expected first response:
- sensitive-information boundary:

### Evidence

- propositions requiring support:
- accepted evidence types:
- provenance and version fields:
- freshness / invalidation rules:
- reviewer qualification:
- disagreement and adjudication:
- storage, access, retention:

### Decision

- outcomes:
- decision authority and delegation:
- quorum if applicable:
- conditions, exceptions, and residual-risk semantics:
- turnaround objective:
- communication and effective date:
- expiry and renewal:

### Follow-through

- action owner and due-date rules:
- condition verification:
- escalation and incident path:
- rollback / stop authority:
- closure evidence:
- feedback into policy, controls, tools, and capacity:

## 5. Forums

Create a forum only when a repeated decision requires joint authority or evidence.

| Forum | Distinct decision right | Scope | Decision members | Evidence / challenge members | Pre-read contract | Outcomes | Service objective | Record / follow-through |
|---|---|---|---|---|---|---|---|---|
| `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` |

Attendance does not equal approval. Record the authorized decision and any dissent explicitly.

## 6. Ownership and assurance

| Responsibility | Accountable role | Required authority | Evidence of operation | Backup / transfer rule |
|---|---|---|---|---|
| Product / use-case outcome | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` |
| Technical system | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` |
| Data | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` |
| Model / platform / tool | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` |
| Control operation | `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` |
| Independent review | `[TBD]` | challenge / assurance, not delivery ownership | `[TBD]` | `[TBD]` |
| Release / residual risk | `[TBD]` | `[TBD]` | decision record | `[TBD]` |
| Incident and remediation | `[TBD]` | stop / contain / recover | exercises and incidents | `[TBD]` |
| Redress / correction | `[TBD]` | correct outcome and downstream effect | case review | `[TBD]` |

## 7. Lifecycle evidence

| Stage | Decision | Minimum evidence | Hard gates | Follow-through |
|---|---|---|---|---|
| Intake | route / reject / request discovery | intended use, owner, preliminary context | prohibited use / missing owner as applicable | discovery owner and due date |
| Discovery | continue / stop / redesign | user need, consequence model, feasibility uncertainty | non-negotiable constraints | evidence plan |
| Pilot | enter bounded exposure | behavior contract, evaluation, controls, incident and stop path | defined by actual authority and harm | pilot conditions and expiry |
| Expansion / release | expand / hold / roll back | pilot outcomes, slices, operations, residual risk | current hard gates | monitoring and invalidation triggers |
| Operation | continue / adjust / pause / retire | outcomes, incidents, change, complaints, control health | stop triggers | remediation / renewal |
| Retirement | decommission / transfer | dependency, data, memory, access, user-impact plan | retention and legal obligations | verification of removal |

## 8. Exceptions and residual risk

Define:

- who may authorize deviation;
- required rationale and alternatives;
- scope and duration;
- compensating controls;
- monitoring and stop triggers;
- expiry and renewal evidence;
- where accepted residual risk is recorded;
- when repeated exceptions trigger redesign.

## 9. Metrics and review

Do not optimize “approval rate” or “gate pass rate” without context.

| Metric | Decision use | Owner | Interpretation / gaming risk | Review cadence |
|---|---|---|---|---|
| time waiting for evidence | capacity and requirement redesign | `[TBD]` | excludes requester delay? | `[TBD]` |
| rework caused by unclear intake or evidence rules | improve service contract | `[TBD]` | requires cause coding | `[TBD]` |
| decisions after useful-by date | authority and capacity issue | `[TBD]` | distinguish deliberate defer | `[TBD]` |
| expired conditions / exceptions | control follow-through | `[TBD]` | stale records may distort | `[TBD]` |
| incidents and recurrence by control path | control effectiveness | `[TBD]` | reporting culture affects count | `[TBD]` |
| decisions invalidated by untracked change | change-control quality | `[TBD]` | detection improves count initially | `[TBD]` |
| duplicate / low-value reviews | remove governance burden | `[TBD]` | qualitative review required | `[TBD]` |

## 10. Improvement review

For selected real cases, ask:

- Was the decision made at the correct level and in time to matter?
- Was the evidence decision-relevant, current, and reusable?
- Which uncertainty or dissent was hidden?
- Which control failed or created false assurance?
- Which exception repeated?
- Which users, affected groups, or incidents were invisible?
- Which forum, artifact, or review could be removed?
- What policy, tooling, staffing, or ownership change follows?

## 11. Open design decisions

| Decision | Owner | Evidence needed | Due | Status |
|---|---|---|---|---|
| `[TBD]` | `[TBD]` | `[TBD]` | `[TBD]` | open / decided / deferred |
