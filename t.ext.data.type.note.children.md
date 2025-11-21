---
id: yipo2qru40ug8bsmnc8svzq
title: Children
desc: ''
updated: 1763064026511
created: 1689993307027
---

Children of a note are defined based on the lowercase [[t.ext.data.type.note.name]].

For example, `a1.a2` is a child of `a1`.

#### Note & children
<details>
<summary>A note can have multiple children, and children can have the same name (in multi-vault scenarios).</summary>

In this example we have the following notes:
- a1 (vault1)
- a1.a2 (vault1)
- a1.a2.a3 (vault1)
- a1 (vault2)
- a1.a2 (vault2)
- a1.a2.a3 (vault2)

The 2 children of a1 are: a1.a2 (vault1) and a1.a2 (vault2)

![img](./assets/images/Screenshot_2023-07-21_at_7.36.41_PM.png){max-width: 300px}
</details>

<details>
<summary>A note can be childless.</summary>

In this example we have the following notes:
- a1 (vault1)
- a1.a2 (vault1)
- a1.a2.a3 (vault1)
- a1 (vault2)
- a1.a2 (vault2)
- a1.a2.a3 (vault2)

Notes a1.a2.a3 (vault1) and a1.a2.a3 (vault2) are childless.

![img](./assets/images/Screenshot_2023-07-21_at_7.36.41_PM.png){max-width: 300px}
</details>


#### Children vs Descendants
Children are direct children of a note, while [[t.ext.data.type.note.descendants]] include all levels below the note in the [[hierarchy|t.ext.data.type.note.hierarchy]].

#### Thorg hierarchy
<details class="bordered-when-open">
<summary>Thorg hierarchy</summary>

![[t.ext.data.type.note.hierarchy]]
</details>
