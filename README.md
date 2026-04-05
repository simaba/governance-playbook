# Enterprise AI Governance Playbook

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/simaba/enterprise-ai-governance-playbook)](https://github.com/simaba/enterprise-ai-governance-playbook/commits/main)

An end-to-end operating playbook for enterprise AI — from intake and prioritisation through release, monitoring, and continuous improvement.

---

## Why this exists

Many organisations experiment with AI without a disciplined operating model. Projects are approved without clear criteria, released without structured gates, and abandoned without retrospectives.

This playbook connects the full lifecycle into a coherent operating system — embedding Lean Six Sigma discipline into AI governance.

---

## Playbook lifecycle

```mermaid
flowchart LR
    A[Intake] --> B[Prioritisation]
    B --> C[Delivery governance]
    C --> D[Release readiness]
    D --> E[Post-release monitoring]
    E --> F[Improvement loops]
    F --> A
```

---

## What's included

### Playbook phases

| Phase | Document |
|-------|---------|
| Intake | `playbook/intake.md` |
| Prioritisation | `playbook/prioritization.md` |
| Release | `playbook/release.md` |
| Monitoring | `playbook/monitoring.md` |
| Improvement | `playbook/improvement.md` |

### Lean Six Sigma integration

| Topic | Document |
|-------|---------|
| AI operating model | `lean-six-sigma/ai-operating-model.md` |
| Metrics and CTQs | `lean-six-sigma/metrics-and-ctqs.md` |

### Templates

| Template | Use for |
|----------|--------|
| `templates/intake-form.md` | Capturing AI project requests |
| `templates/prioritization-matrix.csv` | Scoring and ranking initiatives |
| `templates/improvement-review.md` | Post-release retrospectives |

---

## Companion repositories

- **[AI Release Governance Framework](https://github.com/simaba/ai-release-governance-framework)** — deep-dive on release gates
- **[AI Release Readiness Checklist](https://github.com/simaba/ai-release-readiness-checklist)** — operational checklist for the Release phase
- **[LLM-powered Lean Six Sigma](https://github.com/simaba/LLM-powered-Lean-Six-Sigma)** — AI tool for the Improvement phase

---

## Related repositories

This repository is part of a connected toolkit for responsible AI operations:

| Repository | Purpose |
|-----------|---------|
| [Enterprise AI Governance Playbook](https://github.com/simaba/enterprise-ai-governance-playbook) | End-to-end AI operating model from intake to improvement |
| [AI Release Governance Framework](https://github.com/simaba/ai-release-governance-framework) | Risk-based release gates for AI systems |
| [AI Release Readiness Checklist](https://github.com/simaba/ai-release-readiness-checklist) | Risk-tiered pre-release checklists with CLI tool |
| [AI Accountability Design Patterns](https://github.com/simaba/ai-accountability-design-patterns) | Patterns for human oversight and escalation |
| [Multi-Agent Governance Framework](https://github.com/simaba/multi-agent-governance-framework) | Roles, authority, and escalation for agent systems |
| [Multi-Agent Orchestration Patterns](https://github.com/simaba/multi-agent-orchestration-patterns) | Sequential, parallel, and feedback-loop patterns |
| [AI Agent Evaluation Framework](https://github.com/simaba/ai-agent-evaluation-framework) | System-level evaluation across 5 dimensions |
| [Agent System Simulator](https://github.com/simaba/agent-system-simulator) | Runnable multi-agent simulator with governance controls |
| [LLM-powered Lean Six Sigma](https://github.com/simaba/LLM-powered-Lean-Six-Sigma) | AI copilot for structured process improvement |

---

*Shared in a personal capacity. Open to collaborations and feedback — connect on [LinkedIn](https://linkedin.com/in/simaba) or [Medium](https://medium.com/@bagheri.sima).*
