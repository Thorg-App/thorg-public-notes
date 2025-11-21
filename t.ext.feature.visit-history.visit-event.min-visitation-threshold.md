---
id: uuopjd9qtf8raq8b6dreoll
title: Min Visitation Time Threshold
desc: ''
updated: 1762693847667
created: 1756914894465
---

**Min Visitation Threshold**: The amount of time you need to spend focused in a note for it to be recorded as a `FOCUS` [[visit event|t.ext.feature.visit-history.visit-event]] (default: 3 seconds).

**Use case**: Avoid polluting [[t.ext.feature.visit-history]] with rapid `FOCUS` and `UNFOCUS` events when you rapidly iterate through tabs without stopping to do any meaningful interaction with a note.

**Example**: If you rapidly open notes without spending time in them, by default we will NOT record `FOCUS`.

### How to configure 
See [[t.ext.configuration.values.visitHistory.minVisitationFocusTimeMillis]]

### Overridden on note creation
![[t.ext.feature.visit-history.visit-event.min-visitation-threshold.overridden-on-note-creation]]
