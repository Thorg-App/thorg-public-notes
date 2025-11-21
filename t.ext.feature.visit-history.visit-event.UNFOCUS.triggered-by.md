---
id: 1h1jjkdg73oiynddfg5jp2q
title: UNFOCUS triggered-by
desc: ''
updated: 1762893651542
created: 1762892644885
---

[[t.ext.feature.visit-history.visit-event.UNFOCUS]] is triggered when you unfocus the editor view of the [[note|t.ext.data.type.note]] that you had in focus. There are two main categories that trigger unfocus:

- **User action:**
  - Navigating to a different note
  - Navigating to settings
  - Focusing on non-editor view of the note (e.g., Dendron preview)
  - Focusing on a different application (e.g., IntelliJ)
  - Closing VSCode

- **Prolonged user inaction:**
  - If you focus on a [[note|t.ext.data.type.note]] editor and then leave it without any actions (not scrolling or changing cursor position) for a period longer than [[t.ext.configuration.values.visitHistory.autoUnfocusTtlSeconds]], we will [[auto-unfocus|t.ext.feature.visit-history.visit-event.UNFOCUS.auto-unfocus-due-to-ttl]].