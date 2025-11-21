---
id: n3bq0llls6cmup1elt3asdp
title: Sample Inotify Config
desc: ''
updated: 1763514537705
created: 1762466121633
---

#### Increase Inotify Limits

**One-liner using heredoc:**
```bash
sudo tee /etc/sysctl.d/99-inotify.conf > /dev/null <<'EOF'
# Inotify limits for file watching
fs.inotify.max_user_watches = 524288
fs.inotify.max_user_instances = 256
fs.inotify.max_queued_events = 16384
EOF
```

<details class="bordered">
<summary>OR use your editor of choice to edit config file</summary>

You can use your CLI editor of choice vi/nano/... and edit the */etc/sysctl.d/99-inotify.conf* file new limits like the following: (or )

```txt
fs.inotify.max_user_watches = 524288
fs.inotify.max_user_instances = 256
fs.inotify.max_queued_events = 16384
```
</details>


**Apply the changes:**
```bash
sudo sysctl -p /etc/sysctl.d/99-inotify.conf
```

**Verify it worked:**
```bash
sysctl fs.inotify.max_user_watches; \
sysctl fs.inotify.max_user_instances; \
sysctl fs.inotify.max_queued_events
```

