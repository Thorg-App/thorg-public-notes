---
id: qpv82ki9dujubuqmr35xv49
title: javaExecutablePath
desc: ''
updated: 1762475967658
created: 1757539475260
ap: anchor_point.l8sR6TToUVdIi2Q3x1ANx3S8
---

This is the **full** path (`/some/path/bin/java`) to the Java executable that will be used to start [[t.ext.thorgServer]] by the Thorg Visual Studio Code extension.

**Auto-installed by default**: If you accept the default values during [[t.ext.startup.first-startup]], Thorg will automatically install Java and set this value for you - no manual configuration needed. Thorg installs the OpenJDK JRE (Java Runtime Environment) outside your system `$PATH`, so it won't interfere with your existing system setup.

If you opt out of automatic installation, you'll be prompted to enter the path to the Java executable during initial setup. In this case, make sure you enter the FULL path (`/some/path/bin/java`) to your Java installation. The validation prompts will guide you through entering the correct path.

### Required version
![[t.ext.startup.required-java-version]]

### Where is it stored?
Stored in [[t.ext.configuration.values.startupSetup.javaExecutablePath]]
