---
id: 3pswmt3fy6kd82g7zb9rjj4
title: Assign Shortcut to Open a Frequently Visited File - Navigate to Exact Note.
desc: ''
updated: 1763681014435
created: 1749734000516
---

<div class="llm-tag">

#llm.claude-opus-4
</div>

To create a keyboard shortcut to open a specific frequently visited file without searching:

1. [[Open keybindings.json|t.ext.vscode.how-to.change-your-keybindings-json]]
2. Add the following command with the path to your file:
```json
[
  {
    "key": "ctrl+alt+1",
    "command": "vscode.open",
    "args": "/absolute/path/to/your/frequently-visited-note.md"
  }
]
```

<details class="bordered-when-open">
<summary>Note: Use absolute paths</summary>

**Important:** Relative paths have not been reliable so far. Using **absolute paths** has worked well. For example:
- Windows: `"C:/Users/YourName/projects/myfile.js"`
- Mac/Linux: `"/home/username/projects/myfile.js"`
</details>


####  Related Use Cases
- **Using hot-keyed files with search commands**: Combine this with [[t.ext.command.search.quick.in-subtree.all]] or [[t.ext.command.search.quick.in-subtree.visited-since]] by assigning a shortcut to an [[ancestor note|t.ext.data.type.note.ancestor-note]] in the [[note hierarchy|t.ext.data.type.note.hierarchy]]. This lets you quickly search within a particular note hierarchy from anywhere in your workspace.


#### For Searchability
<details class="bordered-when-open">
<summary>For Searchability</summary>

hot files shortcut hot key
</details>
