---
id: rqsf7ko2vdv6zjpd1grn75z
title: updated
desc: ''
updated: 1755735238057
created: 1724976956489
---

The note's `updated` timestamp is derived from the OS filesystem modification time (mtime).

This approach simplifies note management while providing accurate modification tracking. When you save changes to a note file, the OS automatically updates the file's modification time.

### Git Considerations

When checking out files from git, all files may have their modification time set to the checkout time (not their original modification time). To preserve accurate update timestamps, consider using a tool to restore modification times.

![[t.ext.tip.git.restore-modification-time-mtime]]
