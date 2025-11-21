---
id: 3md78ksd9svi0d0eqde310y
title: Parents
desc: ''
updated: 1705890076439
created: 1689993594376
---

Parents of a note are defined based on the lowercase [[t.ext.data.type.note.name]].


<details>
<summary>1. Top-level notes (e.g., a1) will NOT have a parent.</summary>

In this example we have the following notes:
- a1 (vault1)
- a1.a2 (vault1)
- a1.a2.a3 (vault1)
- a1 (vault2)
- a1.a2 (vault2)
- a1.a2.a3 (vault2)

Notes a1 (vault1) and a1 (vault2) do not have parents, while all other notes in this example do.

![img](./assets/images/Screenshot_2023-07-21_at_7.36.41_PM.png){max-width: 300px}
</details>

<details>
<summary>2. A note can have multiple parents (in multi-vault scenarios).</summary>

In this example we have the following notes:
- a1 (vault1)
- a1.a2 (vault1)
- a1.a2.a3 (vault1)
- a1 (vault2)
- a1.a2 (vault2)
- a1.a2.a3 (vault2)

Note a1.a2 (vault1) has 2 parents: a1 (vault1) and a1 (vault2)

![img](./assets/images/Screenshot_2023-07-21_at_7.36.41_PM.png){max-width: 300px}
</details>
