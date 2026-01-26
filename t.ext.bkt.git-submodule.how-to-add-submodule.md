---
id: rfkdncb0uto62gqqfj5lzfr
title: How to Add GIT Submodule
desc: ''
updated: 1767720527455
created: 1767720229803
---

### Bash command for adding submodule
```bash
    git submodule add "${submodule_url:?}" "${path_where_to_add_submodule:?}"
```

Where `submodule_url` would be something like: `git@gitlab.com:your-username/personal-assets.git`  
And `path_where_to_add_submodule` is the local file path under parent git repository where you want the submodule to be added.



### Example use cases for submodule:
- Manage workspace with multiple vaults
- Separate [[t.ext.data.type.vault]] note GIT history from image asset history.