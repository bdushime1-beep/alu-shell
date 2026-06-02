# Shell permissions

This folder contains solutions for the "Shell, permissions" tasks.

Scripts:

- `0-iam_betty`: switch to user `betty` (uses `su betty`).
- `1-who_am_i`: print effective username (`whoami`).
- `2-groups`: print groups the user is part of (`groups`).
- `3-new_owner`: change owner of `hello` to `betty` (`chown betty hello`).
- `4-empty`: create an empty file `hello` (`touch hello`).
- `5-execute`: add execute permission to owner of `hello` (`chmod u+x hello`).
- `6-multiple_permissions`: set owner/group execute and others read (`chmod 554 hello`).
- `7-everybody`: add execute permission for all (`chmod a+x hello`).
- `8-James_Bond`: set owner/group none and others rwx (`chmod 007 hello`).
- `9-John_Doe`: set mode `-rwxr-x-wx` (`chmod 753 hello`).
- `10-mirror_permissions`: set `hello` mode same as `olleh` (`chmod --reference=olleh hello`).
- `11-directories_permissions`: add execute permission to subdirectories only (`chmod a+x */`).
- `12-directory_permissions`: create `my_dir` with mode `751` (`mkdir -m 751 my_dir`).
- `13-change_group`: change group of `hello` to `school` (`chgrp school hello`).
- `14-change_owner_and_group`: change owner to `vincent` and group to `staff` for all files (`chown -R vincent:staff .`).
- `15-symbolic_link_permissions`: change owner/group of `_hello` symlink (`chown -h vincent:staff _hello`).
- `16-if_only`: change owner of `hello` to `vincent` only if currently owned by `guillaume` (uses `stat` + `awk`).

All scripts are two lines long, start with `#!/bin/bash`, end with a newline, and are executable.
