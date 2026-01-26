---
id: udvbjwwpnih8ox8k8g624dz
title: Install Thorg
desc: ''
updated: 1769453718358
created: 1762451483739
---

### Pre-Requisites
<details class="bordered-when-open">
<summary>You are ok with missing functionality</summary>

We are filling in missing functionally to ergonomically run as standalone but for now we also recommend running [Dendron](https://www.dendron.so/) next to Thorg for some of functionality.
</details>

<details class="bordered-when-open">
<summary>You have a few hundred megabytes of RAM to spare</summary>

- Why: We run a JVM service [[t.ext.thorgServer]] to power Thorg's functionality. This enables more advanced search filtering commands like [[t.ext.command.search.quick.in-subtree.visited-since]].
- By default, Thorg server starts with 1GB allocated to Java max heap space. You can lower this in the configuration (see [[t.ext.configuration.values.startupSetup.serverMaxHeapSpaceMB]]).
  - Note: We have successfully run a 10,000 note test workspace (with 80MB of notes) with only 512MB max heap allocated.
  - Also note that while the default max heap space is set to 1GB, this does not mean JVM/ThorgServer will use the full 1GB—it can operate with much less RAM.
</details>


### Installation steps
- Download the [[latest|t.ext.how-to.install-thorg.latest-release]] Thorg release (Or if required due to an issue see: [[t.ext.how-to.install-thorg.previous-releases]])
![[t.ext.how-to.install-thorg.latest-release]]

- Then follow the steps on [[t.ext.how-to.install-thorg.how-to-install-VSIX-file]]

