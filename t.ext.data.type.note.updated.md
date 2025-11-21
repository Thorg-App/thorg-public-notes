---
id: rqsf7ko2vdv6zjpd1grn75z
title: updated
desc: ''
updated: 1755735238057
created: 1724976956489
---

Front-matter stored value that is used by the app to determine when the note was updated.

```yml
---
updated: 1724977062712
...
---
```

You may ask yourself: the file has an update timestamp in its metadata, so why do we need this? The main use case is to differentiate between refactoring updates and actual note updates. For example, a note can contain a link to a different note that gets renamed. In such cases, the file metadata update date would be increased, but we would want to keep the `updated` date as it was. 
