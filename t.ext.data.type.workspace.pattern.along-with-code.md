---
id: ym6ey8qbya7u9w238dqmtac
title: Thorg Workspace Pattern Along with Code
desc: ''
updated: 1767734925991
created: 1767734402181
---

In this pattern, your [[t.ext.data.type.workspace]] lives in the same directory as your code (most aligned with [monorepo](https://en.wikipedia.org/wiki/Monorepo) code workflow). This tightly integrates documentation notes with the repos Git history. However, Even in this case it's recommended to keep your [[vault|t.ext.data.type.vault]] as a separate git repository and to use [[t.ext.bkt.git-submodule]] for your vault. 

Separating the vault as its own git repository while keeping the history synced up through [[t.ext.bkt.git-submodule]] makes it possible to combine the vault with other vaults in a different thorg workspace (see [[t.ext.data.type.workspace.pattern.with-team-vault]]).
