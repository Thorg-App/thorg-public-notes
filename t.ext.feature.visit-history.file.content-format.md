---
id: gos36f970ejrun6glze9asj
title: Visit history file Content Format
desc: ''
updated: 1762574006469
created: 1753912182270
---

The visit history **file contains the [[note id|t.ext.data.type.note.frontmatter.field.id]]** in the file name. Therefore, we do NOT need to duplicate the note id in the events themselves (see [[t.ext.feature.visit-history.file.location]] for details on file location).

The contents of the visit log file are in compact **text** format with the following structure per line:

### Line Structure

```txt
<ACTION_TYPE>:<TIMESTAMP_SINCE_EPOCH_IN_MILLIS>
```

- **ACTION_TYPE**: Has 2 possible values:
  - `F` - [[t.ext.feature.visit-history.visit-event.FOCUS]] event
  - `U` - [[t.ext.feature.visit-history.visit-event.UNFOCUS]] event (when you leave the note)

- **TIMESTAMP_SINCE_EPOCH_IN_MILLIS**: The timestamp when the event occurred, in milliseconds since epoch.

### Example content
```txt
F:1753911954503
U:1753911959100
```

This translates to:
- `F:1753911954503`: Note was focused at timestamp [1753911954503]
- `U:1753911959100`: Note lost focus at timestamp [1753911959100]


### Stored transparently
Per [[t.ext.data.thorg-view-on-data.transparent-data-model]], we use a human-readable format to store data in a transparent (non-proprietary) way. We opted away from JSONL to keep files compact while retaining human readability and ease of parsing, so you can see what is being recorded and parse it if you desire.
