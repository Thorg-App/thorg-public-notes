---
id: lkn2ujqiorlka9tt4cqysuc
title: Troubleshooting Thorg Server Port Is Used by some other process
desc: ''
updated: 1764254885038
created: 1764171331292
---

This is troubleshooting for when **another** process is using the port that the Thorg server is configured to use.

The simplest approach is to change the port Thorg uses by updating [[t.ext.configuration.values.startupSetup.serverPort]], then [[restart VSCode|t.ext.vscode.how-to.reload]].

If you're curious to learn more on this topic, see below:

<details class="bordered-when-open">
<summary>How to find out which process is listening on the port — and kill it (Linux & macOS)</summary>

![[t.ext.troubleshooting.server-port.is-used-by-some-other-process.how-to-find-out-who-is-listening-on-port-and-shut-it-down-linux-mac]]
</details>