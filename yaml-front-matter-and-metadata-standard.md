---
document-type: guide
title: YAML Front Matter and Metadata Standard
status: Approved
version: 1.0
owner: Jason Masters
created-date: 2026-05-28
created-by: Claude Code
last-updated-date: 2026-06-13
last-updated-by: Jason Masters
tags: [yaml, metadata, markdown, standards]
---

# YAML Front Matter and Metadata Standard

## Relationship to the Taxonomy Guide

This document supports the [AI Requirements and Taxonomy Guide](ai-requirements-and-taxonomy-guide.md). That guide defines how to classify and name requirements. This document explains how to implement consistent metadata across all Markdown documents in your project.

Read the taxonomy guide first if you have not already done so.

---

## What YAML Front Matter Is

YAML front matter is a block of structured metadata placed at the very top of a Markdown file. It sits between two lines of three dashes.

```yaml
---
title: My Document Title
status: Draft
version: 0.1
owner: Jane Smith
created-date: 2026-05-28
---
```

When you open this file in a Markdown viewer, the front matter is usually hidden or rendered as a clean metadata panel. It does not appear in the main body of the document. But it is there in the file, readable by tools, search systems, and AI tools.

---

## Why Metadata Helps AI-Assisted Projects

Metadata solves problems that become visible only as projects grow.

Without metadata, a folder of fifty Markdown files is hard to navigate. You cannot easily answer questions like: which documents are still in draft? Which were updated this week? Who owns this document? Which documents relate to the security module?

With consistent metadata, those questions become answerable. More importantly, AI tools can read metadata and use it to give better answers. An AI tool asked to review all approved requirements can do so reliably when every requirement file has a consistent status field. Without it, the tool has to guess.

> [!NOTE]
> Consistent metadata also supports future automation. As your project tooling matures, metadata fields become the inputs that drive dashboards, reports, and status summaries.

---

## Standard Fields

Use the following fields in every Markdown document in your project.

```yaml
---
document-type:
title:
status: Draft
version: 0.1
owner:
created-date: 2026-05-28
created-by:
last-updated-date: 2026-05-28
last-updated-by:
tags: []
---
```

### Field Definitions

| Field | Required | Description |
|---|---|---|
| document-type | Yes | The type of document: guide, template, requirement, decision, issue, index. |
| title | Yes | The full document title. |
| status | Yes | Current lifecycle status. See status values below. |
| version | Yes | Document version number. See versioning below. |
| owner | Yes | The name of the human responsible for this document. |
| created-date | Yes | The date the document was first created. ISO format: YYYY-MM-DD. |
| created-by | No | Who or what created the document. |
| last-updated-date | Yes | The date of the most recent change. ISO format: YYYY-MM-DD. |
| last-updated-by | No | Who or what made the most recent change. |
| tags | No | A list of keywords for search and filtering. |

---

## Status Values

Use these values consistently across all documents.

| Status | Meaning |
|---|---|
| Draft | Written but not yet reviewed or approved. |
| Under Review | In active review. |
| Approved | Reviewed and accepted. This is the baseline version. |
| Deferred | Out of current scope, retained for a future phase. |
| Rejected | Explicitly excluded, with documented rationale. |
| Retired | No longer applicable; superseded or removed. |

---

## Versioning

Use the following version numbering scheme.

| Version | Meaning |
|---|---|
| 0.x | Draft, not yet approved. |
| 1.x | Approved baseline. |
| 2.x | Major revision to an approved baseline. |

Minor increments (1.1, 1.2) apply to small corrections and updates that do not change the substance of an approved document.

---

## Date Format

Always use ISO 8601 date format: YYYY-MM-DD.

Examples: 2026-05-28, 2026-12-01.

Do not use DD/MM/YYYY or MM/DD/YYYY. These formats are ambiguous when documents are shared across teams or systems.

---

## Tags

Tags are optional but useful for filtering and search. Use lowercase, hyphen-separated values.

```yaml
tags: [requirements, security, crm-module, approved]
```

Keep tags consistent across documents. Define a short list of standard tags at the start of a project and add to it as needed.

---

## Related Documents

For documents that are explicitly linked to other documents, add a related-documents field.

```yaml
related-documents:
  - ai-requirements-and-taxonomy-guide.md
  - templates/requirement-template.md
```

---

## Applying Metadata in Practice

The minimum requirement before sharing any document is:

- title: filled in
- status: set to the current status
- version: set to the current version
- owner: a named person

Everything else can be added progressively. Do not let an incomplete metadata block stop you from creating a document. Add the minimum fields first and complete the rest as the document matures.

---

## Version History

| Version | Date | Author | Summary |
|---|---|---|---|
| 0.1 | 2026-05-28 | | Initial draft |
| 1.0 | 2026-06-13 | | Initial Version (Approved)) |
