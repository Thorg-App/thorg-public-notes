---
id: sazp0de4dglls4juqw0tyn1
title: Back up $HOME/.thorg
desc: ''
updated: 1757532474410
created: 1757081051462
---

### Recommended: Back Up $HOME/.thorg
It's recommended to back up `$HOME/.thorg` (e.g., via source control), which includes your [[visitation history|t.ext.feature.visit-history]]. This allows you to retain this history for later exploration and share it across machines.

### Tip: Ready to Share Across Machines and Users
By default, files in `$HOME/.thorg` (including [[visit history|t.ext.feature.visit-history]]) are completely **private** and outside the vault (relevant if you share vaults with other people). However, while these files are private, they're also designed to be shared across multiple machines and multiple users.

For example, rapidly changing files such as [[visit history files|t.ext.feature.visit-history.file.location]] are structured so they can be shared across multiple users and across multiple machines under a single user **without causing Git merge conflicts**.

Therefore, once you backup/source-control `$HOME/.thorg`, you can share it with yourself across multiple machines or even with other users.

### If You Aren't Using Git
If you are using Git, this directory will contain an auto-populated `.gitignore`. If you aren't using Git, refer to [[t.ext.file.home-thorg-dir.gitignore]] for information on what is recommended to ignore.