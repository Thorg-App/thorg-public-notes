---
id: n1z4f4vgtbg00dxh7o5cwen
title: Finding Workspace - How thorg determines workspace directory
desc: ''
updated: 1762440007155
created: 1748976526111
---

On startup, Thorg needs to find your [[t.ext.data.type.workspace]] directory.

The workspace directory is expected to be somewhere up the file hierarchy from the starting paths.

The starting paths are determined as follows:

```txt
Starting paths are:
  IF vscode.workspace.workspaceFolders is NOT empty
    vscode.workspace.workspaceFolders
  ELSE
    path-of-the-file-you-have-opened
  END-IF
```

### For now we use `dendron.yml` to find the workspace directory
Thorg walks up the parent file chain and looks for a `dendron.yml` file to identify the workspace directory.

### In the near future we will use the .thorg directory to find the workspace
In the near future, we'll primarily identify the workspace using the [[t.ext.data.type.workspace.thorg-dir]] directory (while continuing to support onboarding based on `dendron.yml`).