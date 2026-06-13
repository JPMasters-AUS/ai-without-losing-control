---
document-type: template
title: Module BRD Template
status: Draft
version: 0.1
owner:
created-date: 2026-05-28
created-by: Claude Code
last-updated-date: 2026-05-28
last-updated-by: Claude Code
tags: [template, brd, module]
---

# [Module Name] BRD

> [!NOTE]
> A module BRD documents one bounded business capability or system component. Keeping each capability in its own document means reviews are focused, updates are targeted, and different people or AI tools can work on different modules without creating conflicts. If a module document is growing very large, the capability is probably too broad and should be split.

## Document Control

| Field | Value |
|---|---|
| Status | Draft |
| Version | 0.1 |
| Owner | |
| Parent Document | [Master BRD](../master-brd-template.md) |
| Related Documents | |
| Created | |
| Last Updated | |
| Reviewer | |
| Review Due | |

## Change History

| Version | Date | Author | Summary of Change |
|---|---|---|---|
| 0.1 | | | Initial draft |

---

## Module Purpose

What this module does and why it exists. One to three sentences. If you need more than three sentences, the scope is probably too broad.

---

## Control Objectives

What governance or assurance outcomes does this module need to achieve? Write each as a specific, testable statement.

- Objective:
- Objective:

---

## Problem Statement

The specific user or business pain this module addresses. Be precise.

---

## Users and Stakeholders

- Primary users:
- Secondary users:
- Stakeholder impacts:

---

## Scope

### In Scope

- Item

### Out of Scope

- Item

---

## Non-Goals

Explicitly state what this module does not do. These are firm exclusions, not deferred items.

- This module does not:
- This module does not:

> [!NOTE]
> Non-goals prevent scope creep and limit implied behaviour when AI tools generate outputs from this document. If it is not listed as a goal, an AI tool may still attempt it. Non-goals make the boundary explicit.

---

## Business Requirements

Use the modular ID format: BR-[MODULE]-[SEQUENCE].

- BR-[MOD]-001:
- BR-[MOD]-002:

---

## Functional Requirements

Use the modular ID format: FR-[MODULE]-[SEQUENCE].

- FR-[MOD]-001:
- FR-[MOD]-002:

---

## Business Rules

Rules that govern behaviour regardless of implementation. These are not features; they are constraints.

- Rule:
- Rule:

---

## User Stories / Use Cases

- As a [user type], I want [goal], so that [outcome].
- As a [user type], I want [goal], so that [outcome].

---

## Data Requirements

### Key Data Objects

List the main data objects this module creates, reads, updates, or deletes.

### Required Fields

List mandatory fields for each key data object.

### Data Quality Rules

Rules governing accuracy, completeness, and consistency.

### Retention

How long data must be retained and under what conditions it is archived or removed.

---

## Security Requirements

### Access

Who can access this module and under what conditions.

### Roles

| Role | Permissions |
|---|---|
| | |

### Confidentiality

Data classification and handling requirements.

---

## Audit and Traceability Requirements

### Logging

What events must be logged and at what level of detail.

### Evidence Links

How records link to source evidence or decisions.

### Approval Trail

What approvals must be recorded and by whom.

---

## AI Requirements and Guardrails

> [!NOTE]
> Complete this section for every module, even where AI has no active role. Stating that AI is not used in this module is as important as defining permitted uses. Without an explicit statement, AI tools may assume involvement.

### Allowed Uses

### Prohibited Uses

### Human Approval Points

Decisions that AI may support but humans must make.

### Output Traceability

What sources must AI outputs be traceable to.

---

## Integration Requirements

### Source Systems

Systems that provide data to this module.

### Destination Systems

Systems that consume data from this module.

### Import and Export

File formats, protocols, and frequency.

---

## Reporting and Outputs

### Reports

### Dashboards

### Alerts

---

## Non-Functional Requirements

### Performance

Response time and throughput expectations.

### Availability

Uptime requirements and maintenance windows.

### Usability

Accessibility standards and usability expectations.

### Scalability

Expected volume growth and how the module must respond.

---

## Failure Modes

Identify the ways this module can fail or produce incorrect outcomes. This supports resilience design.

- Failure mode:
- Failure mode:
- Failure mode:

> [!NOTE]
> Documenting failure modes is not pessimism. It is how you design a system that handles the real world rather than only the ideal case.

---

## Requirement Prioritisation

| ID | Requirement Summary | Type | Priority | Source | Rationale |
|---|---|---|---|---|---|
| BR-[MOD]-001 | | Business Rule | Must | | |
| FR-[MOD]-001 | | Functional | Must | | |

Priority values: Must / Should / Could / Won't
Type values: FR / BR / DR / SR / AR / AIR / CR / IR / RR / NFR

---

## Cross-References

### Related Requirements

- [TYPE]-[MOD]-[SEQ]:

### Related Decisions

- DEC-:

### Related Modules

- [module-name]:

---

## Acceptance Notes

Conditions that must be true before this module is accepted as complete.

- Condition:
- Condition:

---

## Risks, Assumptions, Dependencies

### Risks

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| | | | |

### Assumptions

- Assumption:

### Dependencies

- Dependency:

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
