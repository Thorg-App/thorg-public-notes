---
id: szom4dwtme7gf1ozc80rhkt
title: Add Ctrl+T Thorg Shortcuts
desc: ''
updated: 1762814803281
created: 1762541680405
---

`CTRL+t` is used as the entry point for primary Thorg commands. Think of `CTRL+t` as meaning `Thorg` for most commands you assign under it.

### Pre-Req
- [[CTRL+t has been freed|t.ext._.setup-of-shortcuts.ctrl-t-setup.free-ctrl-t]]

### Add CTRL+t Thorg Shortcuts
Add the following to your [[keybindings.json|t.ext.vscode.how-to.change-your-keybindings-json]]:


```json
  {
    "key": "ctrl+t ctrl+t",
    "command": "thorg.search.quick.all"
  },
  {
    "key": "ctrl+t ctrl+h",
    "command": "thorg.search.quick.visited-since.2-hours-ago"
  },
  {
    "key": "ctrl+t ctrl+d",
    "command": "thorg.search.quick.visited-since.today"
  },
  {
    "key": "ctrl+t ctrl+y",
    "command": "thorg.search.quick.visited-since.yesterday"
  },
  {
    "key": "ctrl+t ctrl+w",
    "command": "thorg.search.quick.visited-since.1-week-ago"
  },
  {
    "key": "ctrl+t ctrl+m",
    "command": "thorg.search.quick.visited-since.1-month-ago"
  },
  {
    "key": "ctrl+t ctrl+e",
    "command": "thorg.search.quick.visited-since.1-year-ago"
  },
```

### Description of Additions
The following are descriptions of the shortcuts added to [[keybindings.json|t.ext.vscode.how-to.change-your-keybindings-json]] above:

- `CTRL+t` + `CTRL+t`:
  - Assigned to [[thorg.search.quick.all|t.ext.command.search.quick.all]] for quick [[search|t.ext.command.search._.search-definition]] across all notes.
  - To remember: Thorg, Thorg Main Command.

- `CTRL+t` + `CTRL+h`:
  - Assigned to [[thorg.search.quick.visited-since.2-hours-ago|t.ext.command.search.quick.visited-since]].
    - Through practice, limiting this shortcut to one hour has proven too restrictive, while 4 hours is too permissive. Logically, this shortcut could also be set to:
      - [[thorg.search.quick.visited-since.1-hour-ago|t.ext.command.search.quick.visited-since]]
      - [[thorg.search.quick.visited-since.4-hours-ago|t.ext.command.search.quick.visited-since]]
  - To remember: Thorg, Hour.

- `CTRL+t` + `CTRL+d`:
  - Assigned to [[thorg.search.quick.visited-since.today|t.ext.command.search.quick.visited-since]]
  - To remember: Thorg, Day.

- `CTRL+t` + `CTRL+y`:
  - Assigned to [[thorg.search.quick.visited-since.yesterday|t.ext.command.search.quick.visited-since]]
  - To remember: Thorg, Yesterday.

- `CTRL+t` + `CTRL+w`:
  - Assigned to [[thorg.search.quick.visited-since.1-week-ago|t.ext.command.search.quick.visited-since]]
  - To remember: Thorg, Week.

- `CTRL+t` + `CTRL+m`:
  - Assigned to [[thorg.search.quick.visited-since.1-month-ago|t.ext.command.search.quick.visited-since]]
  - To remember: Thorg, Month.

- `CTRL+t` + `CTRL+e`:
  - Assigned to [[thorg.search.quick.visited-since.1-year-ago|t.ext.command.search.quick.visited-since]]
  - To remember: Thorg, (Second letter of y)Ear (we aren't using `y` since it's used for yesterday)


### Q&A:
<details class="bordered-when-open">
<summary>Why use visited-since and not updated-since for primary shortcuts?</summary>

![[t.ext._.setup-of-shortcuts.ctrl-t-setup.add-shortcuts.why-favor-visited-since]]
</details>
