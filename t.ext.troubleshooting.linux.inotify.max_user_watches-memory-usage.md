---
id: qr1dzx1u8psfe6e7zfmg36e
title: inotify.max_user_watches Memory Usage
desc: ''
updated: 1763515479248
created: 1762466072788
---

**Per-Watch Cost:**
- **32-bit systems:** ~540 bytes per watch
- **64-bit systems:** ~1 KB per watch

**Example:** With `max_user_watches = 1048576`:
- **Worst case (all watches used):** ~1 GB of kernel memory on 64-bit systems
- **Real-world usage:** Typically much less, as not all watches are actively used

⚠️ **Important:** Inotify uses **kernel memory** which cannot be swapped out. But it only uses memory when the watches are used not when you set the limit.


### Memory is used when you use the watches

```bash
# Setting this limit doesn't use any memory yet
# 
# Memory is only used when watches are actually created
# If you only have 1000 active watches, you're using ~1MB, not 1GB
fs.inotify.max_user_watches = 1048576
```

