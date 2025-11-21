---
id: l01369t583p00x1l9czt9ls
title: descendents
desc: ''
updated: 1762546677166
created: 1762443985300
---

Descendants are notes that appear below a given note in the hierarchy, which is determined by [[t.ext.data.type.note.name]].

For example, if a note is named `project.documentation`, its descendants include:
- `project.documentation.api`
- `project.documentation.api.endpoints`
- `project.documentation.api.authentication`
- `project.documentation.api.endpoints.users` (nested descendant)

Descendants include both direct children (one level below) and all nested levels beneath the note in the hierarchy.

See also: [[t.ext.data.type.note.children]] for direct children only.

Learn more about Thorg hierarchy usage below:

![[t.ext.data.type.note.hierarchy]]