---
id: wfr4vrjs33crfamc8wsb034
title: Context field in Frontmatter
desc: ''
updated: 1762806046869
created: 1745893509911
---

`context` is an optional field in note frontmatter which will be used when gathering context for the note. 

Example value: 

```yaml
---
context: 
  - /some/file/path-1
  - /some/file/path-2
---
```

Context gathering will be used largely to feed LLMs with data.