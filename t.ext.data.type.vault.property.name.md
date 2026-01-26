---
id: ldfcvon2mjj6o0q93asxh0m
title: Vault Name
desc: ''
updated: 1767738541929
created: 1746475828896
ap: 
    kt_impl: anchor_point.7s8pC8qLDKKguJ15hJa7uUrG
    nk_shell: anchor_point.m8ZE4Shwp04JHKp3TTeRRJDt.E
---

The Thorg vault name is simply the name of the folder under your workspace.

To keep things simple, for now there is **NO** separate name configuration for the vault.

### Approaches
<details class="bordered-when-open">
<summary>Q: What if I have different Git repositories with the same name? A: Clone with different local names.</summary>

#### Example:
Let's say you have two repositories from different users that share the same name:
```txt
git@gitlab.com:user-1/public.git
git@gitlab.com:user-2/public.git
```

Cloning these as-is would create conflicting directory and vault names. To avoid this, assign different names when cloning:
```bash 
git clone git@gitlab.com:user-1/public.git ./user-1-public
git clone git@gitlab.com:user-2/public.git ./user-2-public
```

This creates two separate directories and therefore two different vault names:
```
./user-1-public
./user-2-public
```
</details>