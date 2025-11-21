---
id: dlmzh8fzpgfvujmarcr4yvq
title: 'Auto-unfocus: Automatically Records UNFOCUS after a period of inactivity.'
desc: ''
updated: 1762553255345
created: 1757089116548
---

If you open a note and then stop interacting with it, after a period of inactivity we will automatically record an `UNFOCUS` [[visit event|t.ext.feature.visit-history.visit-event]] (default: **180 seconds** of inactivity).

If you keep interacting with a note (including typing, scrolling, or moving the cursor position within the note), we will keep resetting the timer until auto-unfocus occurs.

### How to configure
[[t.ext.configuration.values.visitHistory.autoUnfocusTtlSeconds]]