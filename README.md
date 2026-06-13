---
document-type: index
title: Community Edition README
status: Draft
version: 1.0
owner:
created-date: 2026-05-28
created-by: Claude Code
last-updated-date: 2026-06-13
last-updated-by: Jason Masters
tags: [community-edition, ai-governance, getting-started]
---

# AI-Assisted Work: Community Edition

> [!NOTE]
> **New here? A quick orientation before you start.**
>
> The core documents — including the **[How to Work with AI Without Losing Control](how-to-work-with-ai-without-losing-control.md)** starting guide — are written in **Markdown** (`.md`). When you click one on this page, GitHub displays it as a clean, formatted document — there is nothing to install to read it here.
>
> **Not comfortable with Markdown files yet? Two easy options:**
> - Open the **[`pdf/`](pdf/)** folder for a plain PDF copy of every document — easy to read or print.
> - Or spend a few minutes with **[Working with Markdown (.md) Files](working-with-markdown-files.md)** — a short, plain-language guide that makes Markdown click.

## What This Is

This is a practical framework for anyone using AI tools to run projects, build products, or manage documentation in their business.

It answers one question: how do I stop AI-assisted work from becoming an unmanageable mess?

The framework does not require a technical background. It does not assume knowledge of software development, procurement, or governance theory. It is designed for business owners, operators, consultants, and anyone who works alongside AI tools and wants their work to stay organised, traceable, and under control.

---

## Who This Is For

- Business owners using AI tools to create documents, plans, or systems
- Consultants managing client work with AI assistance
- Small teams adopting AI tools for the first time
- Anyone who has experienced AI-assisted work growing chaotic over time

---

## Why These Documents Are in Markdown (.md)

Every document here is a **Markdown** (`.md`) file — plain text with a few simple formatting marks (you write `**bold**` and it shows as **bold**). We use it because it is future-proof, opens in almost any tool, works everywhere AI tools and version control do, and makes changes easy to track — none of which is true of a Word file locked in one app's format.

If `.md` files are new to you — including how to open one and how to format text — start with **[Working with Markdown (.md) Files](working-with-markdown-files.md)**. It covers the essential formatting and the (mostly free) tools for both Mac and Windows.

---

## What Is Included

### Guides

| Document | Purpose |
|---|---|
| [How to Work with AI Without Losing Control](how-to-work-with-ai-without-losing-control.md) | The starting point. Read this first. |
| [AI Collaboration and Governance Framework](ai-collaboration-and-governance-framework.md) | How to structure roles between humans and AI tools. |
| [Project File Structure](project-file-structure.md) | How to organise your project's files — on GitHub, a cloud drive, or your own computer. |
| [Working with Markdown (.md) Files](working-with-markdown-files.md) | What `.md` files are, essential formatting, and the (mostly free) tools to open and edit them. |
| [AI Requirements and Taxonomy Guide](ai-requirements-and-taxonomy-guide.md) | How to classify and track requirements in AI-assisted projects. |
| [YAML Front Matter and Metadata Standard](yaml-front-matter-and-metadata-standard.md) | How to add lightweight metadata to Markdown documents. |

### Templates

| Template | Purpose |
|---|---|
| [Master BRD Template](templates/master-brd-template.md) | Document the overall scope and objectives of a project or product. |
| [Module BRD Template](templates/module-brd-template.md) | Document one bounded capability or component of a larger project. |
| [FRD Template](templates/frd-template.md) | Functional **and** non-functional requirements for a small or single-capability project (paired with a Master BRD or brief). |
| [Requirement Template](templates/requirement-template.md) | Capture a single requirement in a structured, traceable format. |
| [Technical Design Document Template](templates/technical-design-document-template.md) | Describe **how** the solution will be built to meet the requirements. |
| [Decision Record Template](templates/decision-record-template.md) | Record a material decision so it can be understood later. |
| [Issues Register Template](templates/issues-register-template.md) | Track unresolved questions, concerns, and non-blocking issues. |
| [Handover Template](templates/handover-template.md) | Hand work from one party to another — build to operation, between contributors, or at project close. |

---

## Getting Started

You do not need to read everything first. The shortest path to value:

1. **Read [How to Work with AI Without Losing Control](how-to-work-with-ai-without-losing-control.md).** Plain language, about ten minutes, explains the *why*.
2. **Create a home for your project** — a single folder, on your computer, a cloud drive, or GitHub. [Project File Structure](project-file-structure.md) gives you a layout to copy.
3. **Pick your document set** — small project or large? See "Choosing Your Document Set" below, then copy the templates you need into your folder.
4. **Fill them in as you go.** Leave sections blank where they don't apply yet. The templates are starting points, not forms to finish in one sitting.
5. **Keep two habits from day one:** record material decisions (Decision Record), and write down open questions instead of trusting you'll remember them (Issues Register).

That is enough to start. Come back to the other guides when you want the deeper explanation. New to any of the terms below? See [Key Terms](#key-terms).

---

## Choosing Your Document Set

Scale the documents to the size of the project. You do not need every template — pick the set that matches the work.

**Small or single-capability project**

- **Master BRD** (used lightly) or a short project brief — the business context.
- **FRD** — the functional *and* non-functional requirements in one document.
- **Technical Design Document** — how it will be built.

**Large or multi-capability project**

- **Master BRD** — scope, objectives, principles, and system-wide ("cross-cutting") requirements.
- **Module BRD** per capability — each carries that capability's business, functional, and non-functional requirements.
- **Technical Design Document(s)** — how it will be built.

**Across both:** use the **Requirement Template** to expand any single requirement that needs depth; keep a **Decision Record** and **Issues Register** running; and produce a **Handover** when work passes to someone else or the project closes.

> [!NOTE]
> **Where do non-functional requirements go?** They always travel with the requirements layer — never left floating. In a small project they sit in the FRD's Non-Functional Requirements section. In a large project, system-wide NFRs go in the Master BRD's Cross-Cutting Requirements and capability-specific NFRs go in each Module BRD.

---

## Suggested Reading Order

1. How to Work with AI Without Losing Control
2. AI Collaboration and Governance Framework
3. Project File Structure
4. Working with Markdown (.md) Files
5. AI Requirements and Taxonomy Guide
6. YAML Front Matter and Metadata Standard
7. Templates: as needed

If you are short on time, read document 1 and go straight to the templates. Return to documents 2, 3, and 4 when you need deeper explanation.

---

## How to Use the Templates

Each template is a starting point, not a rigid form. Copy the template, fill in what is relevant, and leave sections blank where they do not apply yet.

The templates include YAML front matter at the top. This is explained in the YAML guide. At minimum, fill in title, status, version, and owner before sharing any document.

---

## How to Adapt This Framework

The framework is intentionally general. You do not need every template or every practice to benefit from it. Start with what solves your immediate problem and add structure as your projects grow.

Four principles that should not be skipped regardless of how lightly you adopt this framework:

- Keep a record of material decisions.
- Track unresolved issues rather than assuming they will resolve themselves.
- Ensure one human is accountable for every output.
- Do not let AI tools resolve material uncertainty without your explicit direction.

---

## Contributing and Suggesting Changes

Suggestions and improvements are welcome. This is a **curated** framework — one maintainer reviews every proposed change, so the documents stay consistent and plain-language. Nothing changes unless it is reviewed and accepted.

You do **not** need to be technical to take part:

- **Simplest:** open an **Issue** on GitHub and describe your idea in your own words.
- **To propose exact wording:** open a **Pull Request** (a suggested edit to your own copy that the maintainer can accept).

Every suggestion is reviewed personally and gets one of three outcomes: **accepted as proposed**, **accepted in principle and then reworded to fit the framework**, or **declined with a brief reason**.

Full step-by-step instructions — including how forks and Pull Requests work for non-technical contributors — are in **[CONTRIBUTING.md](CONTRIBUTING.md)**.

---

## Key Terms

Plain-language definitions of the terms used across this bundle.

| Term | What it means |
|---|---|
| **BRD** — Business Requirements Document | What the project needs to achieve and why, from a business point of view. |
| **FRD** — Functional Requirements Document | The detailed list of what the system must *do*, plus how well it must do it. Used for smaller projects. |
| **Module** | One bounded part of a larger project — a single capability documented and built on its own. |
| **TDD** — Technical Design Document | *How* the solution will be built to meet the requirements. |
| **NFR** — Non-Functional Requirement | How *well* the system must perform — speed, reliability, security, ease of use — as opposed to what it does. |
| **Decision Record** | A short note capturing a material choice and the reasoning, so it can be understood later. |
| **Issues Register** | A running list of open questions and unresolved concerns. |
| **Handover** | A document that lets someone else take over the work without the context in your head. |
| **RACI** | A simple way to show, for each task, who is **R**esponsible, **A**ccountable, **C**onsulted, and **I**nformed. |
| **Repository (repo)** | A project's folder of files. On GitHub it also keeps a history of every change. |
| **Markdown (.md)** | Plain text with light formatting (headings, lists, tables). These documents are all Markdown — readable in any text editor. |
| **YAML front matter** | The small block of labels at the very top of each document (title, status, version). Explained in the YAML guide. |

---

## Licence

This work is licensed under a **[Creative Commons Attribution 4.0 International Licence (CC BY 4.0)](LICENSE)**.

You are free to share and adapt this material for any purpose, including commercially, provided you give appropriate credit. A suggested attribution:

> Based on *AI-Assisted Work: Community Edition* by Jason Masters (JPMasters), licensed under CC BY 4.0. Source: https://github.com/JPMasters-AUS/ai-without-losing-control

---

## Version History

| Version | Date | Author | Summary |
|---|---|---|---|
| 0.1 | 2026-05-28 | | Initial draft |
| 0.2 | 2026-06-09 | Claude Code | Added FRD, Technical Design Document, and Handover templates; added "Choosing Your Document Set" guidance (two tiers + where NFRs live) |
| 0.3 | 2026-06-09 | Claude Code | Added Project File Structure guide; expanded README for non-technical readers (Getting Started steps, Key Terms glossary) |
| 0.4 | 2026-06-09 | Claude Code | Added Working with Markdown (.md) Files guide and a "Why Markdown" section to the README |
| 1.0 | 2026-06-13 |Jason Masters | Initial Version (Approved) |
