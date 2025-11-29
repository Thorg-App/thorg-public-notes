---
id: kw4yxql2cgg72zg64muqeos
title: "Recommendation: One Workspace-Multiple Vaults. Instead of multi-workspace"
desc: ''
updated: 1764441642385
created: 1764441374986
---

**Recommendation:** Use one [[t.ext.data.type.workspace]] with multiple [[vaults|t.ext.data.type.vault]].

**Not Recommended:** Running multiple [[t.ext.data.type.workspace]] instances (which requires multiple [[t.ext.thorgServer]] instances).

**Why multiple workspaces are not recommended:**

This approach is typically unnecessary. The recommendation is to run a single workspace containing all your [[vaults|t.ext.data.type.vault]]. Running multiple workspaces has drawbacks:

1) **Resource overhead:** Requires multiple separate instances of [[t.ext.thorgServer]], consuming more system resources.

2) **Navigation difficulty:** You must remember which VS Code window is running which workspace, making quick navigation between apps cumbersome.

**Better approach:**

Use one [[t.ext.data.type.workspace]] containing multiple [[vaults|t.ext.data.type.vault]]. Organize information using [[hierarchies|t.ext.data.type.note.hierarchy]], then leverage tools like [[t.ext.command.search.quick.in-subtree.all]] to search within specific hierarchies.