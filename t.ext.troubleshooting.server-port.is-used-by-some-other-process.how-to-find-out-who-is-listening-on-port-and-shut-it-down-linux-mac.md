---
id: b4tydli3rwwr1mvcg3ffe8o
title: How to Find Out Who Is Listening on Port and shut it down (Linux & Mac)
desc: ''
updated: 1764442226463
created: 1764254022307
---


Finding out which process is listening on a given port is quite useful.

You can do this with the following commands (using port 7567 as an example).

## Linux & macOS

```bash
# `-i` selects by internet address; `:PORT` filters by port number.
# 
# Note: On Linux, you may need `sudo` to see process names for ports owned by other users.
lsof -i :7567
```

You should get output like:

```txt
COMMAND   PID               USER   FD   TYPE DEVICE SIZE/OFF NODE NAME
java    21564 nickolaykondratyev  216u  IPv6  10185      0t0  TCP localhost:7567 (LISTEN)
```

**PID** is the [Process Identifier](https://en.wikipedia.org/wiki/Process_identifier). In the example above, the PID is 21564.

You can use the PID to shut down the process:

### Graceful shutdown

```bash
# SIGTERM tells the app to shut down gracefully, allowing it to
# execute cleanup code and close resources properly.
# 
# After sending this signal, allow some time for the app to finish
# before resorting to SIGKILL.
kill -SIGTERM 21564
```

### Forceful shutdown

```bash
# SIGKILL immediately terminates the process without allowing
# any cleanup code to run. Use as a last resort.
kill -SIGKILL 21564
```
