---
id: dbbtv5m5mo9uj15npscblqo
title: FOCUS - Visit Event
desc: ''
updated: 1762893833472
created: 1762205797677
---

#### What is a FOCUS event?
`FOCUS`: A [[visit event|t.ext.feature.visit-history.visit-event]] that represents you focusing on the editor view of a particular [[note|t.ext.data.type.note]].

#### When is FOCUS eligible to be persisted?
![[t.ext.feature.visit-history.visit-event.FOCUS.eligible-for-persistence-when]]


#### What is NOT a visit event
<details class="bordered-when-open">
<summary>Rapidly jumping in and out of pre-existing note: Not a visit event</summary>

If you jump into a note for less than the [[minimum amount|t.ext.feature.visit-history.visit-event.min-visitation-threshold]] of time (default is a few seconds) and jump out before the minimum time passes, we will NOT record that as a visit event. From the visitation history, it will appear as if you haven't opened that note at all (unless you just created the note).

</details>

<details class="bordered-when-open">
<summary>Seeing the preview of an embedded note: Not a visit event</summary>

If note-A has note-B [[embedded|t.ext.data.type.note-link.example.embed]] in it and you preview note-A, you will see note-B's contents. However, this is NOT considered a visit to note-B (only a visit to note-A).

You need to navigate to note-B explicitly for it to be considered a visit to note-B.
</details>


#### FOCUS is written to file with UNFOCUS
<details class="bordered-when-open">
<summary>FOCUS is persisted to file with UNFOCUS</summary>

A `FOCUS` visit event is persisted into the [[t.ext.feature.visit-history.file]] when its corresponding [[t.ext.feature.visit-history.visit-event.UNFOCUS]] is processed and persisted.

Therefore, if you want your FOCUS event to be persisted (after it has met [[FOCUS eligibility for persistence|t.ext.feature.visit-history.visit-event.FOCUS.eligible-for-persistence-when]]), you need to trigger an UNFOCUS event, which is triggered by:

![[t.ext.feature.visit-history.visit-event.UNFOCUS.triggered-by]]
</details>
