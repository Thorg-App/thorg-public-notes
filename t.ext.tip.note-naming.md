---
id: u6r7irm2nbowv5yl8phzu5f
title: Note Naming Tips
desc: ''
updated: 1758895820037
created: 1758895323831
---

Tips for naming notes (see [[t.ext.data.type.note.name]]):

- **Keep top-level hierarchy items short** and expand naming as you go deeper.
  - This is currently necessary due to VSCode quick pick limitations, which require truncating search results. See [[t.ext.configuration.values.visualPreferences.vsc_quickPick_maxLabelLength]] to adjust the truncation length.

- **Use singular naming for all notes**, including parent notes that contain groups or lists. While plural naming works technically (similar to namespace design in code), singular naming creates a more visually cohesive and readable structure throughout your system.
  - Examples:
    - Use "Project" instead of "Projects" for a parent note containing multiple projects
    - Use "Task" instead of "Tasks" for a note grouping several tasks
  - Concrete example:
    - ✅ `tech.bash.lang.shell-variable.RANDOM`
    - ❌ `tech.bash.lang.shell-variables.RANDOM`

- **Don't overthink it**. You can refactor later when you have more context.


