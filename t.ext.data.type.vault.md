---
id: 3l69532jaroa8rtzdquul3l
title: Vault
desc: ''
updated: 1754329990200
created: 1690744737879
---

A vault is a **folder** located under your [[t.ext.data.type.workspace]] where you store your [[notes|t.ext.data.type.note]] and supporting assets (e.g., images).

To be considered a valid vault, the folder MUST contain a `root.md` file with an id. See [[t.ext.data.type.vault.id]]

<details class="bordered-when-open">
<summary>Comparison with other software</summary>

#### Like Dendron vault
Thorg vault is similar to [Dendron Vault](https://wiki.dendron.so/notes/6682fca0-65ed-402c-8634-94cd51463cc4/). 

#### Unlike Obsidian Vault
However, [Obsidian Vault](https://help.obsidian.md/vault) is more akin to [[Thorg Workspace|t.ext.data.type.workspace]]. 
</details>

### Vault name
![[t.ext.data.type.vault.name]]

### Vault Id
![[t.ext.data.type.vault.id]]

### Relationships
- [[rel.many-to-many]]:**[[t.ext.data.type.workspace]]**
  - A vault can be part of multiple workspaces, and a workspace can have multiple vaults.
