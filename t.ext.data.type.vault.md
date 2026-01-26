---
id: 3l69532jaroa8rtzdquul3l
title: Vault
desc: ''
updated: 1768859544165
created: 1690744737879
---

![[t.ext.data.type.vault.definition]]

![[t.ext.data.type.vault.requirement]]

![[t.ext.data.type.vault.property]]

--------

### Relationships
- [[rel.many-to-many]]:**[[t.ext.data.type.workspace]]**
  - A vault can be part of multiple workspaces, and a workspace can have multiple vaults. See [[t.ext.data.type.workspace.pattern]]

### Highlighted commands
- [[t.ext.command.workspace.vault.register]] - registers existing vault or creates and registers a new vault with [[t.ext.data.type.workspace]].