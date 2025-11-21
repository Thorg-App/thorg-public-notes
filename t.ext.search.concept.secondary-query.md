---
id: 89ipihnou0xz1dwmz38s7js
title: Secondary Query
desc: ''
updated: 1725314675350
created: 1725314608280
---

A more permissive query issued after the exact search match.

### Use Case
In a search system where users may input partial terms (e.g., "inst" instead of "instructions"), the system initially attempts to find matches using exact terms (keyword search). If this initial search yields fewer than a certain number of results, a secondary, broader search using wildcards is conducted. The `matchType` enum allows the system to label each result with the method used to obtain it.

### Relationships
- [[t.ext.search.concept.matchType]]