---
id: z88pyvjjwhf6jy99y1a4171
title: Embed
desc: ''
updated: 1769625052700
created: 1753912744224
---

## Transclusion (Embedding Notes)

Transclusion lets you pull the content of one note directly into another. Instead of just linking to a note, the referenced note's content appears inline—as if you'd copy-pasted it, but it stays in sync with the source.

### Example

Say you have a note called `some.note-1.md` with useful content you want to reuse.

To embed it in another note, use the `![[...]]` syntax:
```md
![[some.note-1]]
```

When you view the note, the full content of `some.note-1` will appear right there.

### Linking vs. Transclusion

| Syntax | What it does |
|--------|--------------|
| `[[some.note-1]]` | Creates a link to the note (click to navigate) |
| `![[some.note-1]]` | Embeds the note's content inline |

Think of the `!` as "inject this here."