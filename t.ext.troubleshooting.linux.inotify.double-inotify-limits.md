---
id: kb20nwzc4jknpakhraik6ib
title: Double Inotify Limits
desc: ''
updated: 1767920127486
created: 1763516496077
---

This is the simplified approach will double all 3 of your current `inotify` limits on linux.

```bash
curl -fsSL https://raw.githubusercontent.com/Thorg-App/script/refs/heads/main/troubleshoot/linux/inotify/inotify_double_current_limits.sh | bash 
```

While above script is coming from our repository. Still [[t.ext.bkt.review-script-prior-to-running-them]] especially as the above script will require `sudo` access to run to be able to modify your system settings.
