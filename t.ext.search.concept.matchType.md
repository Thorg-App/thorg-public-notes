---
id: 21p33doiwyeefy3sg1ex4yh
title: matchType
desc: ''
updated: 1725311202381
created: 1725308933163
---


**Concept: matchType**

### Purpose
The `matchType` differentiates the source of matches when multiple queries are issued to the index for the same user-provided query. This is particularly useful in scenarios where an initial keyword-based query is followed by a more permissive wildcard-based query if the keyword search returns too few results.

### Key Values

#### Search Related
- **Keyword Match (`SEARCH_KEYWORD`)**: Results that were directly matched using exact terms as provided by the user.
- **Wildcard Match (`SEARCH_WILDCARD`)**: Results that were matched using wildcard queries, which are more flexible but typically slower.

#### Lookup Related
- **`LOOKUP_WILDCARD`**: Results that were retrieved using wildcard lookup.

### Use Case
In a search system where users may input partial terms (e.g., "inst" instead of "instructions"), the system initially attempts to find matches using exact terms (keyword search). If this initial search yields fewer than a certain number of results, a secondary, broader search using wildcards is conducted. The `matchType` enum allows the system to label each result with the method used to obtain it.


