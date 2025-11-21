---
id: 0j9jbeegeekkgh3facwp5tq
title: Note Name
desc: ''
updated: 1749077490273
created: 1689993739135
---

Note name is how you reference other notes using wiki links and how you establish note hierarchies.

### Note name is hierarchy
Note names establish the hierarchy of notes, with dot (`.`) as the delimiter between a parent and child note.

For example, consider these files:
```txt
workspace/.thorg
workspace/vault-1/grandparent.parent.child.md
workspace/vault-1/grandparent.parent.md
```

File `grandparent.parent.child.md` has the note name `grandparent.parent.child` and its parent note name is `grandparent.parent`.


### Note linking
![[t.ext.data.type.note-link.example]]

------------------------------------------------------
### Further notes
<details class="bordered-when-open">
<summary>Hierarchies and Cross vault Hierarchy support</summary>

Note names are most important for hierarchy support and cross vault hierarchies.

For example let's say you have **public-vault** with notes 

```txt
grandparent.parent.child-1.md
grandparent.parent.child-2.md
```

And you want to attach a personal note to this hierarchy in a **personal-vault**, you can do so as follows:

```txt
grandparent.parent.private-child-1.md
```

and `grandparent.parent.private-child-1.md` will become a sibling of `grandparent.parent.child-1` and `grandparent.parent.child-2`.
</details>


