---
name: resource-to-notes
description: Convert raw study resources from a domain's resource/ subfolder or prompt context into concise Obsidian revision notes with tables, wikilinks, and inline Mermaid diagrams. Use when the user provides source material or asks to make notes from a resource.
---

# Resource to Revision Notes

## Steps
1. Read `00-Index/Vault-Map.md` to check whether a note on this topic already exists.
2. Read the provided source material (either pasted in the prompt or located inside `<Domain>/resource/`, e.g., `01-DSA-Coding/resource/` or `06-Career-Interview/resource/`).
3. Extract only high-yield revision material: core logic, mechanisms, formulas/code, trade-offs, complexity, and traps (e.g., TCP vs UDP, Big-O pitfalls, race conditions, edge cases).
4. Place the generated `.md` note directly in the parent domain folder (one level above `resource/`). Keep the original file untouched inside `resource/`.
5. Whenever a visual helps recall (algorithm flow, architecture, decision tree, ML pipeline, logic flow), apply the `svg-diagram` skill to embed a concise inline `mermaid` diagram inside the same `.md` file.
6. Present a brief plan (target `.md` file path, create vs. update) and wait for approval before editing any existing file.
7. Write the note following the `AGENTS.md` skeleton and propose the exact 1-line addition to `00-Index/Vault-Map.md`.