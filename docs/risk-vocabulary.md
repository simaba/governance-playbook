# Practical Risk and Decision Vocabulary

This vocabulary is a practitioner aid for keeping common governance terms distinct across planning, evaluation, release readiness, monitoring, and incident response. It is not a legal, regulatory, safety, or compliance classification system.

## 1. System risk tier

A **system risk tier** describes the overall potential impact of deploying a specific system in its intended context. It should be reviewed when the intended use, affected population, autonomy, data category, tool permissions, or reversibility changes.

| Tier | Illustrative meaning | Typical response |
|---|---|---|
| Low | Bounded, reversible, limited-impact support with meaningful human review | Basic technical review, documented owner, test evidence, rollback/disable path |
| Medium | Customer-facing or operationally important capability with material reliability, data, or workflow impact | Structured risk assessment, evaluation evidence, governance review, monitoring plan |
| High | Regulated, safety-adjacent, high-impact, or difficult-to-reverse capability | Accountable formal decision record, relevant specialist review, robust evaluation, incident readiness, oversight and rollback controls |

A system tier should not be inferred from a single test-case score.

## 2. Scenario severity

A **scenario severity** describes the consequence if one specific test, incident, threat, misuse case, or control failure occurs. It is useful for benchmark cases, red-team scenarios, incident triage, and finding prioritization.

| Severity | Illustrative meaning |
|---|---|
| Low | Local, reversible inconvenience or rework |
| Medium | Material workflow, trust, data, or service impact |
| High | Serious security, privacy, safety, financial, legal, or reliability consequence |
| Critical | Severe, broad, irreversible, or non-negotiable harm boundary; requires immediate escalation or containment |

A critical scenario can exist inside a system whose overall tier is medium. Conversely, a high-tier system may contain routine low-severity test cases.

## 3. Control status

A **control status** reports whether a required mechanism is present and supported by evidence. It should not be replaced by a numeric average.

| Status | Meaning |
|---|---|
| Pass / verified | Required control is present and supporting evidence has been reviewed at the stated scope |
| Evidence pending | The control may exist, but sufficient evidence is not yet available for the stated decision |
| Conditional | The control is incomplete or bounded by a documented condition, owner, and due date |
| Fail / blocked | The required control is absent, ineffective, or contradicted by evidence |
| Not applicable | The control is not relevant, with documented rationale and accountable reviewer |

A failed non-negotiable safety, privacy, security, legal, or access-control boundary should block the relevant decision regardless of an aggregate score.

## 4. Evaluation outcome

An **evaluation outcome** describes what a particular suite, case, or artifact demonstrated under stated conditions. It is not automatically a production approval.

| Outcome | Meaning |
|---|---|
| Prototype check passed | The synthetic or limited-scope artifact met the harness's stated checks |
| Evaluation passed with conditions | The stated scope met thresholds, but limitations, blockers, or required follow-ups remain |
| Evaluation held | Material evidence gaps or failures need resolution before expanding scope |
| Evaluation failed | A stated hard gate or quality criterion did not pass |

Always record the scenario set, data provenance, model/configuration version, evaluator/rubric, tool permissions, environment, run count, and exclusions before comparing outcomes.

## 5. Release decision

A **release decision** is an accountable operational decision made by named owners under an organization-specific process. It should reference but not be replaced by evaluation results.

| Decision | Meaning |
|---|---|
| Approve | Required controls and evidence are accepted for the stated scope; residual risks have named owners |
| Approve with conditions | Specific bounded conditions are accepted with owners, deadlines, monitoring, and a decision authority |
| Hold | Material gaps must be resolved before release or expansion |
| Reject / do not release | Critical or unacceptable risks remain unresolved |

## Minimum decision record

For each material evaluation or release decision, record:

- system and configuration version
- intended use, scope, and prohibited uses
- relevant system risk tier and scenario severities
- required controls and evidence status
- residual risks, conditions, and accountable owners
- monitoring, rollback, escalation, and next review date

## Relationship to other repositories

- `agent-eval` uses scenario results and evaluation evidence.
- `automotive-llm-eval-harness` uses a case-level `safety_sensitivity`, which is scenario severity rather than system tier.
- `release-checklist` and `regulated-ai` use system risk tiers to select illustrative control expectations.
- `harness-bench` uses task/run context and quality scoring for comparison, not release approval.
- `multi-agent-governance` uses system ownership, autonomy, trust, and oversight controls.
