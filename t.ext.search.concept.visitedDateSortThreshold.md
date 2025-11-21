---
id: vlmnvb2tpg9shwalt2wvarg
title: Visited Date Sort Threshold
desc: ''
updated: 1762445361066
created: 1755735295857
---

**Concept: Visit Date Sort Threshold**

### Purpose
The `visitedDateSortThreshold` concept refines search result relevance by re-sorting notes with similar match scores based on their last visited date ([[t.ext.data.type.note.visited]]). This ensures that recently visited notes are prioritized within groups of closely matched results.

### Key Idea

- **Threshold-Based Grouping:**
  Search results are grouped if their match scores fall within a defined similarity threshold. This allows grouping notes with nearly identical relevance scores.

- **Visited Date Sorting:**
  Within each group of similar scores, notes are further sorted by their last visited date, ensuring that the most recently viewed notes appear higher in the results.

### Use Case
This concept is valuable when dealing with search results that have close match scores.

### Example
Consider a scenario where 4 notes have the following match scores and visit dates:

- Note A: Score = 2.0, visited on = 2023-09-01
- Note B: Score = 0.9, visited on = 2023-09-02
- Note C: Score = 0.95, visited on = 2023-09-03
- Note D: Score = 0.5, visited on = 2023-09-04

Let's say we have `visitedDateSortThreshold` set to 0.1. Therefore, notes with match scores within 0.1 difference are eligible for re-sorting based on visit date.

In this example, the search response will be:

1. Note A (least recent visit but highest match score)
2. Note C (most recent visit out of B, C)
3. Note B
4. Note D (most recent visit but low match score)





