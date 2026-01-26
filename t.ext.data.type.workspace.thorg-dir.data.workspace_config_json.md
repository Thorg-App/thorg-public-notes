---
id: owzao3g9z470tvkvcr2aj02
title: $THORG_WORKSPACE/.thorg/data/workspace_config.json
desc: ''
updated: 1769209861435
created: 1767651361379
ap:
  kt: anchor_point.3VpZ6vcBAKDqfeDMZtxIiMm5.E
  ts: anchor_point.FkqmfwslLL6cDPALkCEJKiLy.E
---

This file will contain the workspace configuration.

Primary use-case is to have place to define which folders should be attempted to be recognized as we [[vaults|t.ext.data.type.vault]].

### File format: JSON
```json
{
    "_doc_format__thorg_doc_do_not_edit": "Keys ending in __thorg_doc_do_not_edit describe their sibling key...",
    "_top_level__thorg_doc_do_not_edit": "Configuration of [Thorg Workspace](https://notes.thorg.app/notes/37fx82rdmgup4t2m3bdz145). Full documentation: [$THORG_WORKSPACE/.thorg/data/workspace_config.json](https://notes.thorg.app/notes/owzao3g9z470tvkvcr2aj02)",

    "vaults": {
        "<relative_path_from_workspace_to_vault_in_unix_format>": {
            // vault config, can be empty object
        }
    },
    "vaults__thorg_doc_do_not_edit": "Defines [vaults](https://notes.thorg.app/notes/3l69532jaroa8rtzdquul3l) used by thorg workspace. Keys are relative paths from workspace root to vault directory."
}
```

### Relationships
- [[rel.uses]]:**[[t.ext.bkt.doc-val-json-config-pattern]]**


### For Searchability
<details class="bordered-when-open">
<summary>For Searchability</summary>

workspaceconfigjson
</details>
