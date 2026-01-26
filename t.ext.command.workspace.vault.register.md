---
id: hm9xgs1yt3ap0nno9744iy0
title: thorg.vault.register
desc: ''
updated: 1768846739600
created: 1768595615639
---

Registers a vault to be indexed by Thorg within this [[t.ext.data.type.workspace]].

You can either register an existing vault that was previously [[deregistered|t.ext.command.workspace.vault.deregister]], or create a new vault within this workspace.

#### Registering a pre-existing vault
The vault is added to [[t.ext.data.type.workspace.thorg-dir.data.workspace_config_json]].

#### Creating a new vault
This command performs the following actions to satisfy [[t.ext.data.type.vault.requirement]]:

- Creates a new folder with your chosen name
- Places [[t.ext.data.type.vault.root_md]] in it, giving the vault a [[t.ext.data.type.vault.property.id]]
- Registers the vault in [[t.ext.data.type.workspace.thorg-dir.data.workspace_config_json]]


### Relationships
- [[rel.opposite-of]]:**[[t.ext.command.workspace.vault.deregister]]**