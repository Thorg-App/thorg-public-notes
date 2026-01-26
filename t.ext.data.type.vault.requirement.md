---
id: opbjege15mq7lchgrgk6ewr
title: Vault Requirements
desc: ''
updated: 1767734327064
created: 1767733932665
---

For a folder to be recognized as a vault for a given [[workspace|t.ext.data.type.workspace]] the following requirements must be met:
- Must be registered in [[t.ext.data.type.workspace.thorg-dir.data.workspace_config_json]]
  - Why: So that workspace is aware that we want this folder to be recognized as a vault. This is most useful if you 
- Must contain [[t.ext.data.type.vault.root_md]] with valid globally unique [[t.ext.data.type.note.frontmatter.field.id]]
  - Why: So that we can have globally unique identifier for the vault.