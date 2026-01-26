---
id: 6d6hsst6m2ihg52vcypmk4t
title: Free Ctrl+T
desc: ''
updated: 1762814577540
created: 1762538235777
---

Out of the box, VSCode assigns `CTRL+t` to `workbench.action.showAllSymbols`. You'll need to free and remap this so you can use `CTRL+t` as an entry point for **many** commands rather than just a single command.

#### Step 1: Free "ctrl+t" from Being Tied to a Single Command
- [[Open command palette|t.ext.vscode.how-to.open-command-palette]]
- Type `Preferences: Open keyboard shortcuts (JSON)`

Add the following to the file:
```json
  {
    "key": "ctrl+t",
    "command": "-workbench.action.showAllSymbols"
  },
  {
    "key": "ctrl+t",
    "command": "-editor.action.transposeLetters",
    "when": "textInputFocus && !editorReadonly"
  }
```

#### Step 2: Assign New Shortcut for `workbench.action.showAllSymbols`
The recommended shortcut for `workbench.action.showAllSymbols` is `CTRL+t` + `T` (the second time you press T is without CTRL).

To set this up, add the following to your `keyboard shortcuts (JSON)` file (`keybindings.json`):

```json
  {
    "key": "ctrl+t t",
    "command": "workbench.action.showAllSymbols"
  },
```

This setup will leave `CTRL+t` + `CTRL+t` available for [[t.ext.command.search.quick.all]]. 