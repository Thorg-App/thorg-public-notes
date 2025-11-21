---
id: ngo62jicvfp8ad9acw70ozz
title: CTRL+y Thorg Subtree Search Shortcuts
desc: ''
updated: 1762815286889
created: 1762552421563
---


`CTRL+y` is used as the entry point for Thorg in-subtree search commands. To remember this, think of the `Y` character representing the branching of a tree.

### Pre-Req
- [[t.ext._.setup-of-shortcuts.ctrl-y-setup.free-ctrl-y]]

### Shortcuts Overview

Add the following to your [[keybindings.json|t.ext.vscode.how-to.change-your-keybindings-json]]:

```json
  {
    "key": "ctrl+y ctrl+t",
    "command": "thorg.search.quick.in-subtree.all"
  },
  {
    "key": "ctrl+y ctrl+h",
    "command": "thorg.search.quick.in-subtree.visited-since.2-hours-ago"
  },
  {
    "key": "ctrl+y ctrl+d",
    "command": "thorg.search.quick.in-subtree.visited-since.today"
  },
  {
    "key": "ctrl+y ctrl+y",
    "command": "thorg.search.quick.in-subtree.visited-since.yesterday"
  },
  {
    "key": "ctrl+y ctrl+w",
    "command": "thorg.search.quick.in-subtree.visited-since.1-week-ago"
  },
  {
    "key": "ctrl+y ctrl+m",
    "command": "thorg.search.quick.in-subtree.visited-since.1-month-ago"
  },
  {
    "key": "ctrl+y ctrl+e",
    "command": "thorg.search.quick.in-subtree.visited-since.1-year-ago"
  },
```

### Description of Shortcuts

- `CTRL+y` + `CTRL+t`:
  - Assigned to `thorg.search.quick.in-subtree.all` for quick search across all notes in the current hierarchy.
  - To remember: Subtree, Thorg (All).

- `CTRL+y` + `CTRL+h`:
  - Assigned to `thorg.search.quick.in-subtree.visited-since.2-hours-ago`
  - Searches within subtree for notes visited in the last 2 hours.
  - To remember: Subtree, Hour.

- `CTRL+y` + `CTRL+d`:
  - Assigned to `thorg.search.quick.in-subtree.visited-since.today`
  - Searches within subtree for notes visited today.
  - To remember: Subtree, Day.

- `CTRL+y` + `CTRL+y`:
  - Assigned to `thorg.search.quick.in-subtree.visited-since.yesterday`
  - Searches within subtree for notes visited since yesterday.
  - To remember: Subtree, Yesterday.

- `CTRL+y` + `CTRL+w`:
  - Assigned to `thorg.search.quick.in-subtree.visited-since.1-week-ago`
  - Searches within subtree for notes visited in the last week.
  - To remember: Subtree, Week.

- `CTRL+y` + `CTRL+m`:
  - Assigned to `thorg.search.quick.in-subtree.visited-since.1-month-ago`
  - Searches within subtree for notes visited in the last month.
  - To remember: Subtree, Month.

- `CTRL+y` + `CTRL+e`:
  - Assigned to `thorg.search.quick.in-subtree.visited-since.1-year-ago`
  - Searches within subtree for notes visited in the last year.
  - To remember: Subtree, (Second letter of y)Ear (we used `y` for yesterday).

## Notes
- These shortcuts mirror the [[ctrl+t|t.ext._.setup-of-shortcuts.ctrl-t-setup.add-shortcuts]] shortcut pattern but scope searches to the current note's [[hierarchy|t.ext.data.type.note.hierarchy]].