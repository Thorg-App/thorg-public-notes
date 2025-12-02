---
id: b707frllp0tl4z1k4s03h2z
title: $WORKSPACE/.thorg/tmp/server/instance/server.port
desc: ''
updated: 1764441889976
created: 1745250348151
ap: anchor_point.hhJRhRAZM7nuKJogKXY2FagA.E
---

This file holds the [[t.ext.concept.serverPort]] of the [[t.ext.thorgServer]] that is running for this [[workspace|t.ext.data.type.workspace]].

### Location
Located at `$WORKSPACE/.thorg/tmp/server/instance/server.port` when a Thorg server instance is running for this workspace.

This file is deleted when the server terminates gracefully.

### How Port is Determined
The port is dynamically allocated when the Thorg server starts up. The server finds an available port and writes it to this file.

### Related
- [[t.ext.thorgServer.default-port]]
