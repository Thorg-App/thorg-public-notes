---
id: r8b8k17z92zfneh6x2s7bmc
title: Thorg Workspace pattern With Team Vault
desc: ''
updated: 1767734879339
created: 1767734522602
---

Your main [[t.ext.data.type.workspace]] contains two vaults:

- A **private** [[vault|t.ext.data.type.vault]] that only you can access
- A **team** [[vault|t.ext.data.type.vault]] stored in a separate Git repository, synced and shared among teammates, and published as a webview for the company.

In this pattern your workspace can also pull in multiple team vaults under your workspace if you kept separate vaults per project documentation along with code. (See [[t.ext.data.type.workspace.pattern.along-with-code]]).

To make it easy for teammates to pull in multiple repositories that represents vaults under a single workspace you can setup [[t.ext.data.type.workspace]] to use [[t.ext.bkt.git-submodule]] for the vaults that it tracks, and expect a symlink for **private** vault (since each teammate could have their own private vault that only they can access).