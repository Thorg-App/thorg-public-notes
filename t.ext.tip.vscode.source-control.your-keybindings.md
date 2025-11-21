---
id: om9kqluwhq030w59epcfb9a
title: Source Control your keybindings.json
desc: ''
updated: 1762539363075
created: 1749732415150
---

<div class="llm-tag">

#llm.claude-sonnet-4
</div>

**TLDR:** Source control your `keybindings.json` (keyboard shortcuts) file by symlinking it from the VSCode directory to a directory that holds your environment setup.

## Details

Source control your `keybindings.json` file, which manages your keyboard shortcuts in VSCode. Move the actual file to a `git` repository that holds your environment setup (shell configuration, dotfiles, and utility scripts), then symlink to it from VSCode's settings directory. VSCode continues to operate normally while you gain version control benefits.

## Why Source Control Keybindings When Settings Sync Exists?

While VSCode's built-in Settings Sync can sync keybindings between machines, source controlling them yourself provides multiple advantages:

- **Visibility into changes**: Clearly see changes in the JSON through git diffs.
- **Complete history ownership**: Own the entire file history and know when changes were made.
- **Integration with dotfiles**: Your keybindings become part of your broader development environment setup.
- **Platform independence**: Not tied to a Microsoft or GitHub account for Settings Sync.
- **Rollback capability**: Easily revert to previous configurations if something breaks or when experimenting.

## How to Set It Up

1. **Locate your keybindings.json file**:
   - Windows: `%APPDATA%\Code\User\keybindings.json`
   - macOS: `~/Library/Application Support/Code/User/keybindings.json`
   - Linux: `~/.config/Code/User/keybindings.json`

2. **Move the file to your dotfiles repository**:

  ```bash
  # Example: moving to a dotfiles repo
  mv ~/Library/Application\ Support/Code/User/keybindings.json ~/dotfiles/vscode/
  ```

3. **Create a symlink back to the original location**:
   ```bash
   # macOS/Linux example
   ln -s ~/dotfiles/vscode/keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json
   
   # Windows (run as Administrator)
   mklink "%APPDATA%\Code\User\keybindings.json" "C:\path\to\dotfiles\vscode\keybindings.json"
   ```

4. **Commit to your repository**:
   ```bash
   cd ~/dotfiles
   git add vscode/keybindings.json
   git commit -m "Add VSCode keybindings"
   ```

Now your keybindings are version controlled, and VSCode will continue to read and write to the file through the symlink as if nothing changed from its perspective.