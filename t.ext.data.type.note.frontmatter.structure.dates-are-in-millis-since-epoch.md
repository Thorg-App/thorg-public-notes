---
id: ggp4sgqb41rij5hksimi31k
title: Dates Are in Millis since Epoch
desc: ''
updated: 1685895633814
created: 1685895360737
---

FrontMatter date fields such as:
```
---
...
updated: 1685895360737
created: 1685895360737
---
```

are in milliseconds since epoch.

> An integer value representing the timestamp (the number of milliseconds since midnight at the beginning of January 1, 1970, UTC — a.k.a. the epoch).

Example JavaScript to convert to human-readable format:

```js
var timestamp = 1685894903640;
var date = new Date(timestamp);
console.log(date);
```