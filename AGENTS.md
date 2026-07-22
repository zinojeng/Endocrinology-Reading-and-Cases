# Agent instructions — Endocrinology Reading & Cases

**Read `docs/SDD-fellow-reading-platform.md` before doing anything.** It is the single
source of truth for this repo: architecture, content grammar, QA gates, phased plan.
Start with its §0 ("How to use this document").

## Ground rules

- **Never** stage with `git add -A` or `git add .` — the working tree contains macOS
  `Icon\r` junk files. Add explicit paths only (until SDD task P1-1 lands a `.gitignore`).
- Exam-bank content is **private** and must never enter this public repo (SDD §9.1).
  Run the leak check before any commit that touches quiz/exam material.
- Verbatim `_source/` parses are subject to the owner's §9.2 / §11-Q4 decision — do not
  publish new `_source/` verbatim content until that is resolved.
- Do not alter a clinical claim without flagging it for human review. G8 (attending
  sign-off) is always a human step; stop and ask, never self-approve.
- Content style is normative: follow `docs/CONTENT-STYLE.md` (once it exists; until then,
  SDD §2.4 defines the grammar, learned from Ch.36/42/43/44 in `Williams-Textbook/`).

## When a new chapter PDF arrives

Follow the pipeline in SDD §7.1 (stages S1–S8, gates G1–G8). Once Phase 2 is built,
the entry point is:

```bash
npm run new-chapter -- --number NN --slug ChNN-<Slug> --pdf "<path to PDF>"
```

then work the stages: LlamaParse parse → bilingual EN↔ZH → section split + notes →
chapter README → QA gates (G1–G6) → exam sets (private repo) → **stop and request
owner sign-off (G8)**. Record every gate result in `content/chapters.yml`.

Parsing rule: LlamaParse first; free fallback only if the API is unavailable.

## Current implementation status

- Phases 1–2 of the SDD are **not yet implemented** — `chapters.yml`,
  `tools/new-chapter.mjs`, `tools/validate.mjs`, `docs/CONTENT-STYLE.md`,
  `docs/CHAPTER-PIPELINE.md` do not exist yet. Building them (SDD §8.1–§8.2) is the
  first job; the tables in §7.1 and §7.7 are the spec.
- Open owner decisions live in SDD §11. Q1 and Q4 are blocking — if an answer is not
  recorded there, ask the owner instead of assuming.
