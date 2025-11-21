---
id: n44yr1mk4wfgkbqeprbeef9
title: >-
  thorg.visualPreferences.vsc.quickPick.maxLabelLength: Max Length of VSCode
  Quick Pick Labels (Before Truncation)
desc: ''
updated: 1762890600536
created: 1749082685287
ap: anchor_point.ZVbeczqA7mo9u5Ugr7CW8t3h.E
---

Configuration for the max length of labels within [Quick Picks](https://code.visualstudio.com/api/ux-guidelines/quick-picks) used by Thorg. Labels exceeding this value will be truncated. You can adjust this value based on your VSCode zoom level.

### Likely Questions

#### Why don't we make quick pick wider?
VSCode does not allow changing the width of quick pick. An issue about this has been open for over half a decade:

- [Option to widen the command palette · Issue-85374 · microsoft/vscode](https://github.com/microsoft/vscode/issues/85374) - open since 2019
  - Similar issue has been open since 2017 [Allow to change the width of quick open · Issue-38225 · microsoft/vscode](https://github.com/microsoft/vscode/issues/38225)

#### Why is this a config and not auto-adjusted?
This is a configuration instead of being pre-set and auto-adjusting because the number of characters that fit into quick pick varies based on zoom level, and we haven't found the hook to get the proper zoom ratio from VSCode. We provide a sensible default, but if you work with a more zoomed in/out view, adjust this setting to control label truncation in quick pick.