---
id: 5qzvh50rt0sp8gukyqxfm7w
title: Windows How to Increase Path Length
desc: ''
updated: 1766067796195
created: 1766067572938
---

## Problem
Windows (last I checked even Windows11) comes setup to limit the max path length to about 260 characters. Which is quite problematic if you want to have longer note names.

## Solution: enable long paths
The solution is simple to turn on `LongPathsEnabled` option

### In Powershell (Run as **Administrator**)

**Open PowerShell as Administrator:**
   - Press the `Windows` key (or click the Start button)
   - Type `powershell` in the search box
   - **Right-click** on "Windows PowerShell" in the search results
   - Select **"Run as administrator"** from the context menu
   - Click "Yes" when prompted by User Account Control (UAC)

**Enable long paths** by copying the following command and running it in PowerShell:
```ps1
New-ItemProperty -Path "HKLM:\SYSTEM\CurrentControlSet\Control\FileSystem" -Name "LongPathsEnabled" -Value 1 -PropertyType DWORD -Force
```

**Set long paths flag to true in git config:**
```ps1
git config --system core.longpaths true
```

**REBOOT/RESTART** your computer for settings to take effect.