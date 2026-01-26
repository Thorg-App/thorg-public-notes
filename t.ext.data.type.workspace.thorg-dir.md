---
id: cwa47cpquo4v899advakgt7
title: .thorg Data in Thorg Workspace ($THORG_WORKSPACE/.thorg)
desc: ''
updated: 1767651466198
created: 1747785660751
ap: anchor_point.4or1uHet6I14CUgCaom6M8Ke
---


The **Thorg workspace directory (`$THORG_WORKSPACE/.thorg`)** resides under your [[t.ext.data.type.workspace]] directory and holds **Thorg-specific files** that are typically shared by default when using shared vaults.

---

### Source Control Guidance

We recommend tracking the `$THORG_WORKSPACE/.thorg` directory in source control **with appropriate exclusions**:

When Thorg initializes this directory, it creates the following subdirectories:

- [[t.ext.data.type.workspace.thorg-dir.data]] - ✅ Include in source control.
- [[t.ext.data.type.workspace.thorg-dir.tmp]] - 🚫 Exclude from source control (Thorg will automatically add a `.gitignore` entry for this folder).

### Thorg-related files outside of `$THORG_WORKSPACE/.thorg`
Thorg stores additional files outside of the workspace/vault. See [[t.ext.file.home-thorg-dir]]

### Related 
- [[t.ext.data.thorg-view-on-data.transparent-data-model]]