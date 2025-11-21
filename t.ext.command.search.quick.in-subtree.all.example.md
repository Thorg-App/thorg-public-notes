---
id: slcbed14jbrnp7wximlpqy4
title: Thorg Search In Subtree Example
desc: ''
updated: 1762815109529
created: 1749751721833
tags:
  - llm.claude-sonnet-4
---

## File Structure
```txt
workspace/
├── vault-public/
│   ├── recipes.italian.md
│   ├── recipes.italian.pasta.md
│   ├── recipes.italian.pasta.carbonara.md
│   └── recipes.italian.pasta.carbonara.classic.md
└── vault-private/
    ├── family.traditions.cooking.md
    └── recipes.italian.pasta.grandmas-recipe.md
```


**Public Notes:**
- `recipes.italian` - Main Italian recipes overview
- `recipes.italian.pasta` - Pasta cooking guide
- `recipes.italian.pasta.carbonara` - Carbonara recipe
- `recipes.italian.pasta.carbonara.classic` - Traditional carbonara method

**Private Notes:**
- `family.traditions.cooking` - Personal family cooking traditions (different hierarchy)
- `recipes.italian.pasta.grandmas-recipe` - Secret family recipe

## Search Example

### Current Context
- **Selected Note**: `recipes.italian.pasta`
- **Command**: `thorg.search.quick.in-subtree.all`

### Search Scope
Searches the hierarchy of the current note (`recipes.italian.pasta`):

**Included:**
✅ recipes.italian.pasta (current note)
✅ recipes.italian.pasta.carbonara (child)
✅ recipes.italian.pasta.carbonara.classic (grandchild)
✅ recipes.italian.pasta.grandmas-recipe (child, in different vault)

**Excluded:**
❌ recipes.italian (parent - not included)
❌ family.traditions.cooking (different hierarchy - not included)  
