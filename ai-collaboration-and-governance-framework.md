---
document-type: guide
title: AI Collaboration and Governance Framework
status: Approved
version: 1.0
owner: Jason Masters
created-date: 2026-05-28
created-by: Claude Code
approved-date: 2026-06-09
approved-by: Jason Masters
last-updated-date: 2026-06-13
last-updated-by: Codex
tags: [ai-governance, roles, responsibilities, collaboration]
---

# AI Collaboration and Governance Framework

## Purpose

This document defines how to structure the working relationship between humans and AI tools in a project. It covers who does what, who approves what, and where accountability sits.

It applies whether you are working alone with one AI tool, or running a project with multiple AI tools and multiple team members.

---

## The Core Principle

AI tools may assist, draft, review, challenge, and recommend. Humans remain accountable for all decisions.

This is not a limitation of AI tools. It is a governance principle. Accountability is a human concept. When a client, colleague, regulator, or auditor asks who is responsible for a decision, the answer must be a person.

---

## Roles

### The Accountable Owner (You)

The accountable owner is the person responsible for the project and its outputs. In most small business and consulting contexts, this is the business owner or lead consultant.

Responsibilities:

- Define the project vision, objectives, and priorities.
- Review and approve all outputs before they are used or shared.
- Resolve disagreements between AI tools or team members.
- Make all material commercial, strategic, and design decisions.
- Maintain the decision register.
- Authorise any significant action, publication, or delivery.

Boundaries:

- The accountable owner does not accept AI outputs without review.
- The accountable owner does not delegate final approval to an AI tool.

Decision authority: Final. No document is approved, no action is taken, and no output is shared without the accountable owner's review.

---

### AI Documentation and Project Management Assistant

This role covers AI tools used primarily for drafting, writing, and document creation, and for keeping the project organised and on track. Examples include tools used in conversational or canvas modes for creating plans, briefs, requirements, and reports, and for maintaining the project's working records.

Documentation responsibilities:

- Draft documents, templates, and written outputs as directed.
- Review outputs from other AI tools for completeness and alignment with stated requirements.
- Flag gaps, inconsistencies, or ambiguities in drafts or plans.
- Support testing and review activities by drafting test cases and checklists.

Project management responsibilities:

- Maintain the project plan, task backlog, milestones, and dependencies.
- Track progress and deadlines, and produce concise status updates.
- Maintain the decision register, risk register, and issues / open-questions log.
- Proactively surface slipping tasks, blockers, and emerging risks to the accountable owner.

Boundaries:

- Does not make decisions. Drafts, tracks, and proposes. The accountable owner decides.
- Does not approve its own outputs.
- Does not re-prioritise work or change scope on its own initiative; it proposes options, the owner decides.
- Review comments and status flags are advisory. The accountable owner determines whether they require action.

---

### AI Technical Assistant

This role covers AI tools used primarily for technical work: code, analysis, data processing, system design, and structured technical outputs.

Responsibilities:

- Produce technical outputs based on approved requirements and briefs.
- Review documentation and plans for technical feasibility and internal consistency.
- Identify requirements that are ambiguous, contradictory, or technically undeliverable.
- Flag technical concerns to the accountable owner with a clear explanation.

Boundaries:

- Proposes technical approaches. The accountable owner approves technical decisions.
- Does not change requirements without direction from the accountable owner.
- Does not act autonomously on any step that requires the accountable owner's authorisation.

---

### AI Commercial and Research Assistant

This role covers AI tools used primarily for research and commercial support: market and competitor research, commercialisation analysis, branding, marketing, and preliminary legal, IP, and regulatory research. Examples include tools strong at web-grounded research and synthesis.

Responsibilities:

- Conduct market, competitor, customer, and pricing research, with cited sources.
- Support commercialisation: business-model options, go-to-market approaches, and validation questions.
- Draft branding and marketing material (positioning, naming options, copy) for review.
- Research legal, IP, regulatory, and compliance questions and summarise findings with sources.
- Flag commercial risks, untested assumptions, and gaps to the accountable owner.

Boundaries:

- Does not provide legal, financial, or professional advice. It researches and drafts; a qualified human professional must review and own any such advice.
- Does not make commercial, pricing, or strategic decisions. It proposes; the accountable owner decides.
- Research must be evidence-based and cite sources. Unsupported claims are flagged as such, not presented as fact.
- Does not approve its own outputs.

---

## RACI — Who Does What

This table maps project activities to roles using **R**esponsible (does the work), **A**ccountable (owns the outcome and the decision — always a human), **C**onsulted (reviews and advises), and **I**nformed (kept in the loop).

The tool names are **illustrative examples of one current setup — substitute your own**. Here they mirror a working pattern where two general agents staff the documentation/PM and technical roles and **review each other's work** (the four-eyes principle), and a research-oriented agent staffs the commercial role. Whoever drafts, the other reviews — so for the review activity, R and C swap (shown ⇄).

| Activity | Owner *(you)* | Documentation & PM *(e.g. ChatGPT / Codex)* | Technical *(e.g. Claude)* | Commercial & Research *(e.g. DeepSeek / Perplexity)* |
|---|:--:|:--:|:--:|:--:|
| Vision, objectives, priorities | A / R | C | C | C |
| Requirements (BRD / PRD), personas | A | R | C | C |
| Documentation drafting | A | R | C | – |
| Project management: plan, backlog, status, registers | A | R | C | I |
| Technical architecture & design | A | C | R | – |
| Code development & unit testing | A | C | R | – |
| Independent review of any output (four-eyes) | A | C ⇄ R | C ⇄ R | C |
| Testing & acceptance | A / R | C | C | – |
| Commercialisation & market research | A | I | I | R |
| Branding & marketing | A | C | I | R |
| Legal & IP research / outline † | A | I | I | R |
| Release & deployment (under owner authorisation) | A | C | R | – |
| Final approval / sign-off | A / R | I | I | I |

† Legal and IP outputs are **research and drafting only**. A qualified lawyer must review and own any advice before reliance.

Notes:

- The **owner is Accountable (A) on every row** — accountability never transfers to an AI tool.
- For build and documentation activities, the producing agent is **R** and the other agent is **C**; for the dedicated review activity those roles swap (⇄), which is how the four-eyes check is applied.
- The example here mirrors a probity-style split (documentation/business work via ChatGPT/Codex, technical build via Claude); a project where both agents code would assign them differently. **Replace the example tools with whatever you use — the roles, not the brands, are the point.**

---

## Using Multiple AI Tools

Using more than one AI tool in a project is not about finding the best tool. It is about using different tools for different purposes and using their disagreements productively.

Different tools have different strengths. A tool strong at drafting prose may not be the strongest at technical analysis. A tool that produces thorough structured documents may miss nuances that a different tool flags.

More importantly, asking two tools the same question and comparing their answers is a practical quality check. When they agree, you have more confidence in the output. When they disagree, the disagreement usually means one of three things:

- The question or brief was ambiguous.
- There is a genuine complexity or risk that needs your attention.
- One tool has made an error.

All three of these are worth knowing.

> [!NOTE]
> Disagreement between AI tools is information, not a problem. Treat it as a signal to investigate rather than a reason to pick the answer you prefer.

---

## Separation of Responsibilities

Apply a simple rule: no AI tool approves its own work.

If an AI tool drafts a document, a different tool (or a human reviewer) should review it. If an AI tool produces a technical output, a different tool (or a human) should check it against the requirements.

This mirrors the four-eyes principle used in audit and financial controls. The same logic applies here: independent review catches errors that the producing party cannot see in their own work.

---

## Clarification and Uncertainty

When an AI tool encounters ambiguity, incomplete information, or conflicting requirements, it must not silently resolve that uncertainty through its own assumption.

The correct behaviour is to stop, explain the uncertainty clearly, and ask for direction before proceeding.

As the accountable owner, you should expect this behaviour and require it. If an AI tool proceeds confidently through an obvious ambiguity without flagging it, that is a warning sign, not a sign of competence.

When you receive a clarification request from an AI tool, the right response is one of:

- Provide direct clarification.
- Ask the other AI tool for its view.
- Request more analysis.
- Defer the decision and record it as an open question.

Do not allow material uncertainty to be resolved silently. Silent assumption resolution is one of the most common sources of errors in AI-assisted projects.

---

## Confidence and Its Limits

AI tools often express confidence in their outputs. Treat that confidence with appropriate scepticism.

AI tools can produce incorrect information with high apparent confidence. They can misinterpret context, apply the wrong framework, or state something as fact that is not. A confident tone is not a reliability signal.

The practical implication: review every significant AI output yourself, regardless of how confident the tool sounds. Your review is the control, not the tool's self-assessment.

---

## Escalating Material Concerns

If an AI tool identifies a material concern, risk, legal question, or ethical issue in the course of its work, it must raise that concern with the accountable owner before proceeding. It should not proceed through a known concern on the assumption it will be resolved later.

As the accountable owner, you should treat any such flagged concern seriously, even if the tool's framing seems overly cautious. It is easier to dismiss an unnecessary escalation than to fix a problem that was not raised.

---

## What AI Tools Do Not Do

Regardless of how they are configured, AI tools in this framework do not:

- Make strategic, commercial, or final decisions.
- Approve their own outputs.
- Override the accountable owner's direction.
- Introduce scope, functionality, or approaches not discussed with the accountable owner.
- Guarantee factual accuracy.
- Resolve material uncertainty through silent assumption.
- Provide qualified legal, financial, or professional advice. They assist with research and drafting; a qualified human professional must review and own such advice.

---

## Handoff and Approval Protocol

When a document or output moves from one party to another for review, the transfer should be explicit. An informal mention in a chat does not constitute a handoff.

A simple protocol:

1. The producing party marks the output as ready for review and notifies the reviewer.
2. The reviewer works against that specific version.
3. Review comments go to the accountable owner, who decides what to action.
4. If changes are required, the producing party updates and the process repeats.
5. When satisfied, the accountable owner marks the output as approved.

In practice, a version-controlled repository (such as GitHub) provides a natural handoff mechanism. A commit or push to the repository creates a timestamped, traceable handoff point.

---

## Version History

| Version | Date | Author | Summary |
|---|---|---|---|
| 0.1 | 2026-05-28 | | Initial draft |
| 0.2 | 2026-06-02 | Claude Code | Added project management to the documentation role; added the Commercial & Research role; added a RACI chart with example tool mappings; added the "no professional advice" boundary |
| 0.2 approval | 2026-06-09 | Jason Masters | Approved as the current working framework. Any later CC clarity/example updates should be recorded as a new version. |
| 1.0 approval | 2026-06-13 | Jason Masters | Initial Version for Release|