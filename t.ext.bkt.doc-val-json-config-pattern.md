---
id: nl18br971v7hysee2b0mzh756
title: Doc/Val Json Config Pattern
desc: ''
updated: 1769209856801
created: 1767728194296
---

## High-Level Goal
Enable configuration files to reference their documentation, making it easy for advanced users and Thorg developers to understand configuration options directly from the config files themselves.

## Problem
JSON doesn't support comments, while alternative formats that do (like [JSON5](https://json5.org/)) have limitations:
- **Poor cross-language support** for programmatically writing comments (Kotlin & TypeScript)
- **Lack of robust tooling** like `jq` that advanced users depend on for JSON manipulation

## Proposed Solution: Sibling `__thorg_doc_do_not_edit` Keys
Place a `<key>__thorg_doc_do_not_edit` sibling next to each documented configuration key:

This approach enables:
- Programmatic comment/documentation writing when modifying configs
- In-file documentation references for users
- Preservation of JSON's tooling ecosystem (`jq`, etc.)
- Cross-language compatibility (Kotlin & TypeScript)
- Direct value access without extra nesting

### Example Structure
```json
{
    "_doc_format__thorg_doc_do_not_edit": "Keys ending in __thorg_doc_do_not_edit describe their sibling key...",

    "server": {
        "port": 8080,
        "port__thorg_doc_do_not_edit": "Port the server listens on",

        "timeout": 30,
        "timeout__thorg_doc_do_not_edit": "Seconds before connection fails"
    },
    "server__thorg_doc_do_not_edit": "Top-level server configuration"
}
```

### Future Enhancement
JSON Schema can be added later for validation and editor integration. The `__thorg_doc_do_not_edit` keys provide immediate in-file documentation, while schema adds type checking, autocomplete, and generated docs. Both approaches complement each other.

### Real-World Example
See: [[t.ext.data.type.workspace.thorg-dir.data.workspace_config_json]]
