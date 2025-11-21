---
id: jsfr19a17fji2delxpiwtvm
title: Script to See Which Inotify Limit Is Low
desc: ''
updated: 1763518265453
created: 1763513633889
---

If you ran into inotify issues and want to find out which inotify limit you are running low on you can start with just checking your current limits, with the simple command in bash:

```bash
sysctl fs.inotify.max_user_watches; \
sysctl fs.inotify.max_user_instances; \
sysctl fs.inotify.max_queued_events
```

This should print output that contains something like:
```bash
fs.inotify.max_user_watches = 524288
fs.inotify.max_user_instances = 256
fs.inotify.max_queued_events = 16384
```

If you want to get the actual limits used, that is not as straightforward and requires some scripting. You can see some options [here](https://unix.stackexchange.com/a/502359/364768), (Also remember [[t.ext._.review-script-prior-to-running-them]])