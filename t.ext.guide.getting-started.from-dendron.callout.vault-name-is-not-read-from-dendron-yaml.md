---
id: tyjmcmzgygfacc0812p840u
title: Vault Name Is Not Read from Dendron Yaml
desc: ''
updated: 1748974009997
created: 1748972556959
---


Vault names are **now derived solely from the vault's folder name** and are **no longer** read from `dendron.yml`. (See [[t.ext.data.type.vault.name]])

Most users won't be affected by this change, as vault names usually already match their corresponding folder names. However, if the `name` property in your `dendron.yml` configuration doesn't match your vault's folder name, an adjustment is needed for smooth operation with Thorg.

### How to Adjust (Both Adjustments Are Needed):
<details class="bordered-when-open">
<summary>Adjusting Your Vault's Name in dendron.yml</summary>

Open your `dendron.yml` file (found at the workspace level). You will see a vault configuration similar to this:

```yaml
workspace:
    vaults:
        -
            fsPath: vault-2
            name: second-vault
```

To resolve the mismatch, you have two options:
1. Rename the `name` property to explicitly match the `fsPath` (the vault's folder name).
2. Delete the `name` property entirely.

#### Desired `dendron.yml` Configuration Examples:

```yaml
workspace:
    vaults:
        -
            fsPath: vault-2
            name: vault-2
```

OR simply delete the name property:

```yaml
workspace:
    vaults:
        -
            fsPath: vault-2
```
</details>


<details class="bordered-when-open">
<summary>Adjusting Name in Your VS Code Workspace File (.code-workspace)</summary>

Your VS Code workspace file (e.g., `dendron.code-workspace`) might also contain `name` properties for your vaults under the `folders` array.

Locate your `.code-workspace` file (usually at the workspace root) and find entries similar to this:

```json
{
    "folders": [
        {
            "path": "vault-2",
            "name": "second-vault"
        },
        // ... other folders
    ],
    // ... rest of the config
}
```

To achieve consistency, you have two options:
1. Rename the `name` property to explicitly match the `path` (the folder name).
2. Delete the `name` property entirely.

#### Desired `.code-workspace` Configuration Examples:

```json
{
    "folders": [
        {
            "path": "vault-2",
            "name": "vault-2"
        },
        // ...
    ]
}
```

OR

```json
{
    "folders": [
        {
            "path": "vault-2"
        },
        // ...
    ]
}
```
</details>
