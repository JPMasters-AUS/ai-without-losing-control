---
document-type: template
title: Functional Requirements Document (FRD) Template
status: Draft
version: 0.1
owner:
created-date: 2026-06-09
created-by: Claude Code
last-updated-date: 2026-06-09
last-updated-by: Claude Code
tags: [template, frd, requirements]
---

# [Project or Product Name] — Functional Requirements Document (FRD)

> [!NOTE]
> **When to use this.** The FRD is the requirements document for a **small or single-capability project**. Pair it with a Master BRD (or a short project brief) that holds the business context, and use this FRD for the detailed requirements. For a **large, multi-capability project**, use Module BRDs instead — one per capability — rather than a single FRD.
>
> **This FRD carries both functional *and* non-functional requirements.** A functional-only document is incomplete for build: performance, availability, security, and usability need a home too. They live in the Non-Functional Requirements section below.

## Document Control

| Field | Value |
|---|---|
| Status | Draft |
| Version | 0.1 |
| Owner | |
| Parent / Context Document | [Master BRD or project brief]() |
| Contributors | |
| Created | |
| Last Updated | |
| Reviewer | |
| Review Due | |

## Change History

| Version | Date | Author | Summary of Change |
|---|---|---|---|
| 0.1 | | | Initial draft |

---

## Purpose

Why this document exists and what it governs. One to three sentences. Reference the Master BRD / brief for business context rather than repeating it.

---

## Scope

### In Scope

- Item

### Out of Scope

- Item

> [!NOTE]
> Explicit out-of-scope items are as important as in-scope items. They prevent scope creep and stop AI tools from implying behaviour that was never intended.

---

## Users and Stakeholders

- Primary users:
- Secondary users:
- Stakeholders:

---

## Functional Requirements

The core of the FRD: what the system must do. Use the ID format `FR-[SEQUENCE]` (e.g. FR-001), or `FR-[AREA]-[SEQUENCE]` if you have a few logical areas. Each requirement should be testable.

| ID | Requirement | Priority | Acceptance Criteria | Source |
|---|---|---|---|---|
| FR-001 | | Must | Given … when … then … | |
| FR-002 | | Should | | |

Priority: Must / Should / Could / Won't. Use the [Requirement Template](requirement-template.md) to expand any requirement that needs fuller treatment.

---

## Business Rules

Rules that govern behaviour regardless of implementation. Constraints, not features.

- Rule:
- Rule:

---

## User Stories / Use Cases

- As a [user type], I want [goal], so that [outcome].
- As a [user type], I want [goal], so that [outcome].

---

## Data Requirements

### Key Data Objects

The main data objects this system creates, reads, updates, or deletes.

### Required Fields

Mandatory fields for each key object.

### Data Quality Rules

Accuracy, completeness, and consistency rules.

### Retention

How long data is kept and how it is archived or removed.

---

## Non-Functional Requirements

> [!NOTE]
> These define *how well* the system must perform, as distinct from *what* it does. In a small project they live here, with the functional requirements. (In a large project, system-wide NFRs go in the Master BRD's Cross-Cutting Requirements and capability-specific NFRs go in each Module BRD.)

### Performance

Response time and throughput expectations.

### Availability

Uptime requirements and acceptable maintenance windows.

### Usability and Accessibility

Usability expectations and accessibility standards to meet.

### Scalability

Expected volume growth and how the system must respond.

### Maintainability / Portability

Any constraints on how easily the system can be changed, supported, or moved.

---

## Security and Access Requirements

### Access

Who can access the system and under what conditions.

### Roles and Permissions

| Role | Permissions |
|---|---|
| | |

### Confidentiality

Data classification and handling requirements.

---

## AI Requirements and Guardrails

> [!NOTE]
> Complete this even where AI has no role. Stating that AI is *not* used is as important as defining permitted uses — otherwise an AI tool may assume involvement.

### Allowed Uses

### Prohibited Uses

### Human Approval Points

Decisions AI may support but a human must make.

### Output Traceability

What sources AI outputs must be traceable to.

---

## Integration Requirements

- Source systems:
- Destination systems:
- Import / export formats, protocols, frequency:

---

## Reporting and Outputs

- Reports:
- Dashboards:
- Alerts / notifications:

---

## Failure Modes

How the system can fail or produce incorrect outcomes, so resilience can be designed in.

- Failure mode:
- Failure mode:

---

## Acceptance Criteria

Conditions that must be true before this is accepted as complete.

- Condition:
- Condition:

---

## Cross-References

- Related decisions (DEC-):
- Related issues (ISS-):
- Related requirements:

---

## Risks, Assumptions, Dependencies, Constraints

### Risks

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| | | | |

### Assumptions

- Assumption:

### Dependencies

- Dependency:

### Constraints

- Constraint:

---

## Open Questions

| Question | Owner | Due | Resolution |
|---|---|---|---|
| | | | |

---

## Approvals

| Name | Role | Decision | Date |
|---|---|---|---|
| | | Draft / Approved / Approved with Conditions / Deferred / Rejected | |
