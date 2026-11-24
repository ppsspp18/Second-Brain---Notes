---
name: vault-curator
description: Audit the Obsidian vault for missing wikilinks, orphan notes, unprocessed files in resource/ folders, Mermaid syntax issues, and out-of-date Vault-Map entries. Use when the user asks for vault maintenance, suggestions, or a revision health check.
---

# Vault Curator

## Steps
1. Scan all `.md` revision notes directly inside `01-DSA-Coding/`, `02-CS-Fundamentals/`, `03-System-Design/`, `04-ML-DL/`, `05-AI-Engineering/`, and `06-Career-Interview/` (exclude files inside `*/resource/` from the revision note list).
2. Compare all revision notes against `00-Index/Vault-Map.md`.
3. Check every `*/resource/` folder for raw files that have not been converted into revision notes yet.
4. Scan `mermaid` code blocks for common syntax bugs (unquoted brackets/parentheses or colons inside node labels).
5. Output a concise audit table listing:
   - Notes missing from `Vault-Map.md`
   - Unprocessed files waiting in `*/resource/`
   - Broken `[[wikilinks]]` or malformed `mermaid` blocks
   - High-value cross-links between related notes
6. Do NOT edit, rename, or delete any file until the user approves specific items.