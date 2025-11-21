---
id: 204kbxavabzre3vkydtnapi
title: Quick Search In Subtree
desc: ''
updated: 1763064347273
created: 1749491286928
command_id: thorg.search.quick.in-subtree.all
ap: anchor_point.G6WXJZfRhtzrZ6OGsiVc819k
---

<div class="command-definition">

Search all notes in the **[[subtree|t.ext.data.type.note.subtree]]** of the currently selected/opened [[note|t.ext.data.type.note]].
</div>

### Command ID
```txt
thorg.search.quick.in-subtree.all
```

### Behavior
- **Includes current note** → Yes
- **Includes descendant notes** → Yes
- **No note selected** → Warning message

### Example
<details class="bordered-when-open">
<summary>Usage Example</summary>

![[t.ext.command.search.quick.in-subtree.all.example]]
</details>

### Also see
#### Shortcuts
- [[t.ext._.setup-of-shortcuts.ctrl-y-setup]]

#### Related Tips
![[t.ext.command.search.quick.in-subtree._.tip]]
 
#### Related Commands
- [[t.ext.command.search.quick.in-subtree.visited-since]] - Like quick search in subtree, but also filters by [[last visited|t.ext.data.type.note.visited]] before performing the [[search|t.ext.command.search._.search-definition]].
- [[t.ext.command.search.quick.in-subtree.updated-since]] - Like quick search in subtree, but also filters by [[last updated|t.ext.data.type.note.updated]] before performing the [[search|t.ext.command.search._.search-definition]].