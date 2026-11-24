---
name: revision-condense
description: Compress verbose or messy notes into concise revision sheets with comparison tables, key takeaways, and inline Mermaid diagrams. Use when the user asks to shorten, summarize, clean up, or make a note revision-ready.
---

# Revision Condenser

## Steps
1. Read the target `.md` note completely.
2. Identify bloated paragraphs, repeated explanations, or long prose steps that compress better into a Markdown table or an inline `mermaid` flowchart.
3. Show a brief before/after structural plan and ask permission before overwriting the note.
4. Rewrite the note for a 60–90 second revision scan:
   - Keep formulas, complexity (`O(...)`), edge cases, and core code patterns intact.
   - Replace prose comparisons with Markdown tables and multi-step logic with concise inline `mermaid` blocks.
   - Preserve all valid existing `[[wikilinks]]`.
5. End with the `Suggestions` block from `AGENTS.md`.