---
id: 37fx82rdmgup4t2m3bdz145
title: Thorg Workspace
desc: ''
updated: 1768859567520
created: 1690744774869
---

A functioning workspace is a collection of one or more [[vaults|t.ext.data.type.vault]].

In practice this is a folder containing all the files necessary to manage your information in Thorg. 

In thorg documentation this directory will be referred to as `$THORG_WORKSPACE`.

The suggested usage pattern is to have a single main `$THORG_WORKSPACE` that can include multiple [[vaults|t.ext.data.type.vault]]. Allowing each [[vault|t.ext.data.type.vault]] toe be independently versioned and included in differently configured workspaces.

## Typical layout
Typical layout will be as follows:

```
$THORG_WORKSPACE/
    /$VAULT_1
    /$VAULT_2
    /.thorg
    /other-directories and files...
```

## Sub-directories
- In typical setup one level down will be [[vaults|t.ext.data.type.vault]], which to be recognized as vaults need to meet [[t.ext.data.type.vault.requirement]].

## Patterns
![[t.ext.data.type.workspace.pattern]]

