---
id: 5wq691vs7bkjf59xd629c3l
title: Note id in frontmatter
desc: ''
updated: 1763063510419
created: 1743465009741
---

The ID in frontmatter is the minimum value needed to deem a markdown file as a parseable note.

### Format
```yaml
---
id: <globally-unique-string>
---
```

```yaml
---
id: 5wq691vs7bkjf59xdsdsadf
---
```

### Why is `id` required?

#### Stable links
Without an `id`, whenever you publish (web view), you would publish with the file name. This makes the links very brittle if any refactoring occurs. We want to allow linking to published notes in a much more stable fashion, so you can refactor note hierarchies without breaking links to your published views.

#### Long-term metadata
A globally unique, **stable** identifier tied to the file allows us to store metadata about that note, such as [[t.ext.feature.visit-history]].