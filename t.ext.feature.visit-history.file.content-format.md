---
id: gos36f970ejrun6glze9asj
title: Visit history file Content Format
desc: ''
updated: 1768678900000
created: 1753912182270
---

[[t.ext.feature.visit-history.file]]: contains the data to power [[Visit history Feature|t.ext.feature.visit-history]] (in short this file contains the timestamps of when you visited particular note).

[[Visit history file path|t.ext.feature.visit-history.file.location]] **contains the [[note id|t.ext.data.type.note.frontmatter.field.id]]** in the file name. Therefore, we do NOT need to duplicate the note id in the events that we store.

The contents of the visit history file are in compact **text** format with the following structure per line:

### Line Structure (VisitPair format)

```txt
<FOCUS_TIMESTAMP_MILLIS>:<DURATION_MILLIS>
```

- **FOCUS_TIMESTAMP_MILLIS**: When the [[t.ext.feature.visit-history.visit-event.FOCUS]] event occurred (milliseconds since epoch).
- **DURATION_MILLIS**: How long the visit lasted (milliseconds).

Each line represents a **complete visit** (a FOCUS followed by UNFOCUS).

### Example content
```txt
1753911954503:4597
1753912000000:60000
```

This translates to:
- `1753911954503:4597`: Visit started at timestamp [1753911954503], lasted [4597] ms (~4.6 seconds)
- `1753912000000:60000`: Visit started at timestamp [1753912000000], lasted [60000] ms (1 minute)

### Stored transparently
Per [[t.ext.data.thorg-view-on-data.transparent-data-model]], we use a human-readable format to store data in a transparent (non-proprietary) way. We opted away from JSONL to keep files compact while retaining human readability and ease of parsing, so you can see what is being recorded and parse it if you desire.

### Future-proof parsing guidance

<details class="bordered-when-open">
<summary>Future-proof parsing guidance</summary>

If you're parsing this data, you can future-proof your implementation by expecting additional fields to be added after the current ones, separated by the `:` delimiter.

In future versions, we may extend the data recorded per visit:

```txt
1753911954503:4597:<some-new-data>:<additional-field>
```

**Simple future-proofing strategy:**
1. Take one line
2. Split on `:` delimiter to get tokens
3. Read `tokens[0]` (focus timestamp) and `tokens[1]` (duration)
4. Ignore any additional tokens beyond index 1

This ensures your parser continues working even as new fields are added.
</details>