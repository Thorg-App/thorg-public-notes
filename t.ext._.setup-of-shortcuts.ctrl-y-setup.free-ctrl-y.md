---
id: 5lutxtlee7y1ttx3ju0jfnn
title: Free Ctrl+Y
desc: ''
updated: 1762814568961
created: 1762552101702
---

Out of the box, VSCode assigns `CTRL+y` to `redo`. You'll need to free and remap this so you can use `CTRL+y` as an entry point for **many** commands rather than just a single command.

#### Step 1: Free "ctrl+y" from Being Tied to a Single Command
- [[Open command palette|t.ext.vscode.how-to.open-command-palette]]
- Type `Preferences: Open keyboard shortcuts (JSON)`

Add the following to the file:
```json
  {
    "key": "ctrl+y",
    "command": "-chatEditor.action.acceptHunk",
    "when": "chatEdits.hasEditorModifications && editorFocus && !chatEdits.isRequestInProgress || chatEdits.hasEditorModifications && notebookCellListFocused && !chatEdits.isRequestInProgress"
  },
  {
    "key": "ctrl+y",
    "command": "-redo"
  }
```

#### Step 2: Assign New Shortcut for `redo`
The recommended shortcut for `redo` is `CTRL+y` + `Y` (the second time you press Y is without CTRL).

To set this up, add the following to your `keyboard shortcuts (JSON)` file (`keybindings.json`):

```json
  {
    "key": "ctrl+y y",
    "command": "redo"
  }
```

This setup will leave `CTRL+y` available as an entry point for multiple commands.
