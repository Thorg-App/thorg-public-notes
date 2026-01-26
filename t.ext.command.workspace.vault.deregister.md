---
id: 1b22fik4xbcs7dpuo12n906
title: thorg.workspace.vault.deregister
desc: ''
updated: 1768846778926
created: 1768595717035
ap:
  kt_int_api_interface_for_action: anchor_point.PndlDCyfp8sG9ye83t7kVxNm.E
  kt_int_api_interface_for_list_of_choices: anchor_point.36dj3iqzvHitr5bOXfobotG4.E
  kt_integ_test: anchor_point.pSOUiH9GC2I6E2Po5PGSW28K.E
---

De-registers the vault from [[t.ext.data.type.workspace]] by removing the vault path from [[t.ext.data.type.workspace.thorg-dir.data.workspace_config_json]].

**This command does NOT delete files.** It only changes the configuration so that Thorg stops processing the vault. You can add the vault back by running [[t.ext.command.workspace.vault.register]].


### Relationships
- [[rel.opposite-of]]:**[[t.ext.command.workspace.vault.register]]**