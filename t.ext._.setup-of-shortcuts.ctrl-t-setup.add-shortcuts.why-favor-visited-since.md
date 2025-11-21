---
id: unwobg6slfsie92l4gss9iu
title: Why use visited-since and not updated-since for primary shortcuts
desc: ''
updated: 1762547330452
created: 1762545424540
---

#### Why Use Visited-Since and Not Updated-Since as Primary Shortcuts?

##### Visited Encompasses Modified for Most Cases
We choose [[visited-since commands|t.ext.command.search.quick.visited-since]] over [[updated-since|t.ext.command.search.quick.updated-since]] because if you perform modifications on a note, you'll likely stay in that note longer than your configured [[t.ext.feature.visit-history.visit-event.min-visitation-threshold]]. Therefore, your visit will be recorded as a [[t.ext.feature.visit-history.visit-event]] for the modified note and will be picked up by [[visited-since commands|t.ext.command.search.quick.visited-since]].

##### Updated-Since Does Not Encompass Visited Notes
You could visit and stay at a note for a prolonged period **without** making modifications or updates. In such cases, the note will be fresh in your memory and likely related to the area you're currently working on. A note that has been read has a higher chance of being re-visited, and it's picked up by [[visited-since|t.ext.command.search.quick.visited-since]] commands. However, such a note that has been read but not modified is out of reach of [[updated-since|t.ext.command.search.quick.updated-since]] commands.


#### Also see
- [[t.ext._.setup-of-shortcuts.ctrl-t-setup.add-shortcuts.why-favor-visited-since.when-updated-since-can-be-better]]