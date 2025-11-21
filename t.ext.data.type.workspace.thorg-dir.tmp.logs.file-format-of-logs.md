---
id: xvahd3ritqcmxewfrfp4ccy
title: File Format of Log Files
desc: ''
updated: 1763162549498
created: 1763162429840
---

### Format
```txt
<log_type>.<UTC_DATE>.log

# If the logs are rotated within the same date there will be rotation suffix
<log_type>.<UTC_DATE>.log.[ROTATION_SUFFIX_NUMBER]
```

### Example
```txt
vsc_client.2025_11_12.log
vsc_client.2025_11_12.log.1
```