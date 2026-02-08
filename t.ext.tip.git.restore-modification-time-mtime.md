---
id: az0q4n5khzojm0s59vg3vfs
title: Restoring File Modification Times After Git Checkout
desc: ''
updated: 1738717200000
created: 1738717200000
---

When files are checked out from git, their modification time (mtime) is set to the checkout time rather than their original modification time. This affects features that rely on file modification times, such as "updated since" search filters.

### Solution: git-restore-mtime

The `git-restore-mtime` tool restores file modification times based on git commit history.

### Installation

```bash
# Ubuntu/Debian
sudo apt install git-restore-mtime

# macOS (via Homebrew)
brew install git-restore-mtime

# pip (cross-platform)
pip install git-restore-mtime
```

### Usage

After checking out a repository or branch:

```bash
git restore-mtime
```

### Example: Bash Function

```bash
git.restore_modification_mtime () {
    echo.func "${@}";
    local dir="${1:-${PWD:?}}";
    git -C ${dir:?} restore-mtime || {
        echo.yellow "Failed to restore modification time.";
        return 1
    }
}
```

### When to Use

- After `git clone`
- After `git checkout` (switching branches)
- After `git pull` (if files were modified)
- Before using Thorg's "updated since" search filters
