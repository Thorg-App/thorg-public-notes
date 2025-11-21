---
id: gqq49b4y8p6y1qhlc780877
title: thorg.logs.capture.combined.recent - Command To capture Recent logs
desc: ''
updated: 1763755087182
created: 1763740678932
ap: anchor_point.wCk4USdUcy2tc4CxecTpxmHf.E
---

Command to capture recent Thorg logs by combining multiple log files into a single file based on a date range.

**Use case:** Instead of [[getting Thorg logs manually|t.ext.contact-us.submit-git-hub-issue.how-to.submit-logs.how-to-get-logs.manually]], use this command to simplify log gathering. 

This command prompts you for a time range and gathers logs from multiple files (pre-init, client, and server) based on your specified range.

**Note:** If your issue is reproducible, we recommend enabling `DEBUG` level logging in [[t.ext.configuration.values.advancedConfig.logLevel]].

### How to use
1. [[Open the command palette|t.ext.vscode.how-to.open-command-palette]]
2. Type **Capture combined logs** and select **Thorg/Logs: Capture Combined Logs (Recent)**
3. Choose the date range from the quick pick menu
   1. Example if the issue happened at activation time you only need to gather the logs since activation (first option).
4. Wait for the log gathering report showing the combined log file location
