---
id: s0967vprvghxe9a712v2ipw
title: Manually get Thorg logs
desc: ''
updated: 1763740633341
created: 1763740538396
---


You can manually collect thorg logs by going through 2 main locations for Thorg logs:

- [[t.ext.file.home-thorg-dir.not-under-scm.logs]] - Contains initialization/pre-startup logs. These are logs that occur before we found [[t.ext.data.type.workspace]] directory and before we're able to get [[t.ext.thorgServer]] up and running. If you're having initialization issues, please share the logs from this directory.
- [[t.ext.data.type.workspace.thorg-dir.tmp.logs]] - This is where the main logs are stored from both the server and client. If the issue happened post-initialization, logs from this directory should be sufficient.