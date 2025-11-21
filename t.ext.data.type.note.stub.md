---
id: dnlltvp0top7xbckks6bikx
title: Stub Note
desc: ''
updated: 1762818015786
created: 1689994827416
---

A stub note is an in-memory creation (without writing files). Stubs mainly exist to help with navigation and to make it easier to create missing notes in the hierarchy. 

This is best explained with an example. Let's say you have the following real notes:
- a1
- a1.a2.a3-I
- a1.a2.a3-II
- a1.a2.a3-III
- a1.b2.b3-I
- a1.b2.b3-II
- a1.b2.b3-III

Two stubs will be created in the above scenario:
- a1.a2
- a1.b2

These stubs help with navigation so that instead of having 6 notes directly under note `a1`, `a1` now has 2 children: `a1.a2` and `a1.b2`. Each of these in turn has 3 children of their own. `a1.a2` has `a1.a2.a3-I`, `a1.a2.a3-II`, and `a1.a2.a3-III`, while `a1.b2` has `a1.b2.b3-I`, `a1.b2.b3-II`, and `a1.b2.b3-III`, making the hierarchy much more manageable.

### Characteristics of a stub note:
- A stub cannot be a leaf note.
- A stub must have a descendant that is a real file note.
  - If all stub children are removed, the stub note disappears.
- A stub can have a stub as a child. Inversely, a stub can have a stub as a parent.
  - As long as there is a descendant leaf that is a real note.