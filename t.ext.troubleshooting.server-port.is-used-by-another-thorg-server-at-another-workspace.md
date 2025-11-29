---
id: r1o92483gdtavwi9zminuhp
title: "Troubleshooting: Port Is Used by Another Thorg Server at Another Workspace"
desc: ''
updated: 1764442347418
created: 1764440317209
---

This error occurs when another [[t.ext.thorgServer]] instance is already running on the same port but in a different [[t.ext.data.type.workspace]].


### If you're running a single workspace and got this error

Even after closing all VS Code instances, you may still encounter this error. This typically means a Thorg server instance did not shut down properly.

Refer to [[t.ext.troubleshooting.server-port.is-used-by-some-other-process.how-to-find-out-who-is-listening-on-port-and-shut-it-down-linux-mac]] for operating system-level steps to identify and shut down the misbehaving server process.

### If you want to run multiple workspaces (not recommended)

If you still want to run multiple [[t.ext.data.type.workspace]] instances simultaneously after reading [[t.ext.tip.thorg.one-workspace-multiple-vaults]], you'll need to change the port number for one of the workspaces.

To do this, modify the [[t.ext.configuration.values.startupSetup.serverPort]] setting in one of the running workspaces.