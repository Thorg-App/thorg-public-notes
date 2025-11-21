---
id: cqgcad6pqaiwysbesyijq4n
title: Visit History file Location - (Where visit history data is written to)
desc: ''
updated: 1763729500255
created: 1753919412638
ap:
  a_main: anchor_point.IEg0FX995sL6plSzWEEniHwz
  location-test-ap: anchor_point.T1TIHEHKkvGh7vIf8mzJpC4k
---
 
### Location
```txt
$HOME/
  .thorg/
    usr/
      {user_name}/
        qc/
         h/
            v/
              vid_{vault_id}/
                {machine_name}/
                  nid_{note-id}.visit_log
```

- `$HOME/` - Your user directory.
- `.thorg/` - Thorg directory under your home folder ([[t.ext.file.home-thorg-dir]]).
- `usr/` - Stands for split by thorg username.
- `{user_name}/` - [[t.ext.concept.thorgUsername]]
- `qc/` - Stands for *quick changing*.
- `h/` - Folder stands for *history*.
- `v/` - Folder stands for *visit*.
- `vid_{vault_id}/` - [[t.ext.data.type.vault.id]]
- `{machine_name}/` - [[t.ext.concept.machineName]]
  - Machine name exists to prevent merge conflicts when you share your visit history for the same user across multiple machines.
- `nid_{note-id}.visit_log` - Visit log for the [[t.ext.data.type.note]], indexed by [[note_id|t.ext.data.type.note.frontmatter.field.id]].
  - By including the note id in the file name, we avoid storing the note id within the events themselves (see [[t.ext.feature.visit-history.file.content-format]]).

### Recommendation
![[t.ext.file.home-thorg-dir._.banner-for-descendent-dirs-to-be-backed-up]]