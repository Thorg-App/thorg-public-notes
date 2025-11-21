---
id: mdrrjqvzi3vdajr9r3rac0i
title: Dive Deeper and Set Inotify by Hand
desc: ''
updated: 1763515523376
created: 1763515514337
---


<details class="bordered">
<summary>Overview</summary>

On Linux, file system monitoring relies on the [Inotify](https://en.wikipedia.org/wiki/Inotify) facility. Inotify requires a *watch handle* for each directory being monitored. For intelligent IDEs like IntelliJ, VSCode, and Thorg, detecting external file changes is essential for knowing the state of files of interest.

</details>


### Troubleshooting

There are couple of different `inotify` limits that you might need to increase. The following script can help you figure out which limit you are breaching.

![[t.ext.troubleshooting.linux.inotify.script-to-see-which-limit-is-low]]

After running the above script you can adjust your limits by editing your system *inotify* configuration values:

![[t.ext.troubleshooting.linux.inotify.sample-inotify-config]]


### References

- [Inotify Watches Limit Linux | JetBrains Knowledge Base](https://youtrack.jetbrains.com/articles/SUPPORT-A-1715/Inotify-Watches-Limit-Linux)
- [Linux Kernel Inotify Increase commit](https://github.com/torvalds/linux/commit/92890123749bafc317bbfacbe0a62ce08d78efb7)
- [Inotify Wikipedia](https://en.wikipedia.org/wiki/Inotify)
