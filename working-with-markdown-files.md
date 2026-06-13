---
document-type: guide
title: Working with Markdown (.md) Files
status: Draft
version: 1.0
owner: Jason Masters
created-date: 2026-06-09
created-by: Claude Code
last-updated-date: 2026-06-13
last-updated-by: Jason Masters
tags: [markdown, getting-started, tools, formatting]
---

# Working with Markdown (.md) Files

Every document in this bundle is a **Markdown** file — a file ending in `.md`. If you have not used Markdown before, this guide explains what it is, why we use it, how to format text in it, and what (mostly free) tools open and edit it.

---

## What Markdown Is

Markdown is **plain text with a few simple formatting marks**. You write `**bold**` and it displays as **bold**. You start a line with `#` and it becomes a heading. That is essentially all there is to it.

A `.md` file is just a text file. You can open one in any text editor and read it without anything special — the formatting marks are designed to be readable even before they are "rendered" into nicely styled output.

---

## Why We Use It

For AI-assisted work, Markdown has real advantages over a Word document:

- **It is future-proof.** Plain text opens in anything, on any system, decades from now. It is never locked inside one company's app or file format.
- **It is readable as-is.** Even with no special software, the content is legible.
- **It works everywhere.** Every editor, every AI tool, and every version-control platform (like GitHub) reads and writes it natively. AI tools in particular produce Markdown by default.
- **Changes are easy to track.** Because it is plain text, you (or GitHub) can see exactly what changed between two versions — which matters for the decision and version discipline this framework encourages.
- **It separates content from styling.** You focus on *what* you are writing; the rendering decides how it *looks*. The same file can become a web page, a PDF, or a printed document.

The trade-off is that it is less familiar than Word and has fewer point-and-click formatting buttons. This guide closes that gap.

---

## Essential Formatting

### Always works (standard Markdown)

| To get… | Type this | Result |
|---|---|---|
| *Italic* | `*italic*` or `_italic_` | *italic* |
| **Bold** | `**bold**` | **bold** |
| ***Bold italic*** | `***bold italic***` | ***bold italic*** |
| Headings | `# Heading 1`, `## Heading 2`, `### Heading 3` (down to `######`) | section headings, large to small |
| A line across the page | `---` on its own line | a horizontal rule |
| Bulleted list | `- item` (one per line) | a bullet list |
| Numbered list | `1. item` (one per line) | a numbered list |
| Link | `[text to show](https://example.com)` | a clickable link |
| Image | `![description](path/to/image.png)` | an embedded image |
| Quote | `> quoted text` | an indented blockquote |
| Inline code | `` `code` `` | `code` in monospace |
| New paragraph | leave a blank line between blocks | a paragraph break |

### Widely supported (most modern tools)

These are "GitHub-Flavored Markdown" extensions — supported almost everywhere, but technically additions to the core.

| To get… | Type this |
|---|---|
| Table | `\| Col A \| Col B \|` then a separator row `\|---\|---\|`, then your rows |
| ~~Strikethrough~~ | `~~strikethrough~~` |
| Checkbox / task list | `- [ ] to do` and `- [x] done` |

### May need an add-in — or use the HTML fallback

These are the ones you flagged. Support varies by tool (Pandoc and Obsidian handle them; many simpler editors do not). Where a tool does not support the Markdown form, a plain **HTML tag works as a fallback in almost every renderer.**

| To get… | Markdown form (if supported) | Reliable HTML fallback |
|---|---|---|
| Superscript (x²) | `x^2^` | `x<sup>2</sup>` |
| Subscript (H₂O) | `H~2~O` | `H<sub>2</sub>O` |
| Footnote | `Some text.[^1]` … and later `[^1]: the note.` | (no simple HTML equivalent — needs a tool that supports footnotes, e.g. Pandoc/Obsidian) |
| ==Highlight== | `==highlight==` | `<mark>highlight</mark>` |
| Underline | (no standard Markdown) | `<u>underline</u>` |

> [!NOTE]
> If a formatting feature you need is not rendering, two fixes usually work: (1) switch the tool's setting or extension on, or (2) drop in the HTML tag shown above. HTML is valid inside Markdown.

---

## Tools to Write Markdown

> [!NOTE]
> The tools below are **examples to show the range of choices — not recommendations or endorsements.** Platforms and pricing change, so check current details before choosing. Each category has free and paid options; pick what fits your budget and comfort.

**Free — already on your computer**

- **TextEdit** (Mac) — set it to *Plain Text* mode (Format → Make Plain Text) and save as `.md`.
- **Notepad** (Windows) — plain text by default; save with a `.md` extension.
- These work but show no live preview — you see the raw marks, not the rendered result.

**Free — purpose-built (cross-platform: Mac and Windows)**

- **Visual Studio Code** — free; has a built-in Markdown preview (open it side-by-side). Very widely used.
- **Obsidian** — free for personal use; a Markdown-based notes/knowledge system (this is what the vault these documents live in uses).
- Open-source editors such as **Zettlr**, **MarkText**, **Ghostwriter**, **Joplin**, or **Logseq** — all free.

**Paid — polished writing experiences**

- **Typora** — Mac/Windows/Linux; a clean "what you see is what you get" editor; one-time purchase, free trial.
- **iA Writer** — Mac/Windows; distraction-free; one-time purchase (per platform).
- **Ulysses** — Mac/iOS; subscription.

---

## Tools to View / Preview Markdown

Often you do not need a separate viewer — **most of the editors above render a live preview themselves** (VS Code, Obsidian, and Typora all show formatted output as you type).

If you do want a dedicated viewer:

- **Marked 2** (Mac) — a paid, one-time-purchase previewer that watches a file and shows it beautifully rendered; pairs with any plain editor.
- **Windows** — there is no single famous equivalent, but options include VS Code's or Obsidian's preview, dedicated apps such as **MarkdownPad** (free and paid versions), or a browser extension (below).
- **Any web browser** — add a free "Markdown Viewer" extension (available for Chrome, Edge, Firefox) and you can open `.md` files straight in the browser.
- **GitHub / GitLab** — if your files live there, they render `.md` automatically in the browser, no software needed.

---

## Where Word and Pages Fit (Not Well)

**Microsoft Word and Apple Pages are not Markdown tools.** They save their own formats (`.docx`, `.pages`) and do not write Markdown marks. You *can* work around this, but with caveats:

- **Export to plain text, then rename to `.md`:** this only gives you the words. Word/Pages will not insert the `#`, `**`, or table syntax, so a bold heading just becomes ordinary text — you would have to add the Markdown marks by hand afterward. Fine for a quick capture; poor for a real document.
- **Proper conversion with a converter:** a free, open-source tool called **Pandoc** converts `.docx` to `.md` (and back) while keeping the structure. It is a command-line tool, so slightly technical; there are also one-off online converters for occasional jobs.

**Bottom line:** if you only occasionally need to bring a Word document across, convert it with Pandoc. If you are creating these documents regularly, it is far easier to write directly in a free Markdown editor such as Visual Studio Code or Obsidian than to fight Word into shape.

---

## The Reassuring Summary

- A `.md` file is just text — you cannot really "break" it.
- You already have a tool that opens it (TextEdit or Notepad).
- For a nicer experience, a free editor with live preview (VS Code or Obsidian) is the easiest upgrade.
- You only need to remember a handful of marks — bold, italic, headings, lists, links, tables — to do almost everything in this bundle.

---

## Version History

| Version | Date | Author | Summary |
|---|---|---|---|
| 0.1 | 2026-06-09 | Claude Code | Initial draft |
| 1.0 | 2026-06-13 | Jason Masters | Initial Version (Approved) |
