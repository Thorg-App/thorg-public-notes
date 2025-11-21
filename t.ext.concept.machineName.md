---
id: e2utao7fadssxpunp5tqy7m
title: Machine Name
desc: ''
updated: 1762453414393
created: 1757536804698
ap:
  _ts: anchor_point.V9FTQwxLHVIkmnbWzinTNeRu
  kt: anchor_point.QXC2lB3w3RQEIggplGBIfWFq
---

### What is it?
*machineName*: A name for your machine that is unique under your chosen username.

Valid examples: [`macos-laptop-1`, `windows-desktop`, `machine-1`]


### Why it exists?
Primary use case: to disambiguate changes made on different machines while using the same username. This prevents unnecessary Git merge conflicts in data such as [[t.ext.feature.visit-history]]. Thorg segments the files it creates using the *machineName* you provide. 

### Avoid sharing this value across machines
Do NOT share or re-use this value across machines. Sharing it will cause Git merge conflicts in your [[t.ext.feature.visit-history]]. 

### Example scenario
#### Starting scenario
You have a **laptop** and **desktop** that you use. Valid values for *machineName* would be "laptop" and "desktop" respectively.

#### IF you got a 2nd laptop for prolonged usage
If you need a 2nd laptop while retaining your previous laptop, a valid value for *machineName* on the brand new laptop would be "laptop2".

#### IF you got a 2nd laptop without overlap in usage
If you sold your laptop and don't plan any overlap in usage between the old and new laptop, it's OK to give the new laptop the designation "laptop" for *machineName*.


### When do you specify it?
You will specify it during the initial start up of Thorg.

### Where is it stored?
In [[t.ext.configuration.values.startupSetup.machineName]]


