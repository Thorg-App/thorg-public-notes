---
id: 3x0492fmyozxjiywq9b81u7
title: Common Thorg Workspace Patterns
desc: ''
updated: 1769209754242
created: 1767653445141
---

## Main patterns for [[workspaces|t.ext.data.type.workspace]]
### Pattern 1: Main workspace - At Home (Recommended to start with)
This is the recommended pattern to start with as it's the simplest to set up and preserves your Git history as you move [[notes|t.ext.data.type.note]] between [[vaults|t.ext.data.type.vault]].

In this pattern, you have a **single** Git repository for your [[workspace|t.ext.data.type.workspace]] containing one **private** vault. This means you only have one Git repository to manage initially. You can create additional vaults under the workspace, and they'll be source controlled as well. Git history is retained as you move files between vaults, provided the vaults are part of this workspace's repository and you commit moves separately from content changes (so Git can detect file similarity).

### Pattern 2: Main Workspace — At Home - Public Repo as Separate Vault
Your main `$THORG_WORKSPACE` contains a **private** [[vault|t.ext.data.type.vault]] in one Git repository (accessible only to you) and a **public** vault published as a webview in a separate Git repository. 

- PRO: Separate repository for public vault that is ready to be shared as GIT repository.
- CON: Moving notes from public to private looses their edit GIT history as the repositories are separate.

### Pattern 3: Main Workspace — At Work
![[t.ext.data.type.workspace.pattern.with-team-vault]]


### Pattern 4: Workspace Along with code
![[t.ext.data.type.workspace.pattern.along-with-code]]

## Optional Add-on Patterns (Intermediate/Advanced)

These patterns are optional and can be combined with the setups above.

### Add-on Pattern 1: [[t.ext.bkt.git-submodule]] for Assets

**Why**: Keeps your main repository's Git history clean by separating out images and other assets.

**How**: Create a separate Git repository for each vault's assets (e.g., a **private** vault would have a corresponding **private-assets** repository). Then add this repository as a submodule at `$VAULT/assets/submodule`. See [[t.ext.bkt.git-submodule.how-to-add-submodule]] for details.

**Pros**:
- Keeps Git histories separate while maintaining a clear relationship between repositories
- Allows you to track exactly which asset commits correspond to which main repository commits

**Cons**:
- Adds complexity to your workflow
- Requires familiarity with Git submodule commands