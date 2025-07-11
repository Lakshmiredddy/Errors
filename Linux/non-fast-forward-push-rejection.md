## ERROR:

$ git add . ; git commit -m "linux" ; git push origin main
[main b07debe] linux
 3 files changed, 83 insertions(+)
 create mode 100644 linuxkey
 create mode 100644 linuxkey.pub
 create mode 100644 ssh_keys_for_new_user.md
To https://github.com/Lakshmiredddy/Linux.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Lakshmiredddy/Linux.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

## SOLUTION:
* It is happened beacause remote branch having updates that local branch doesn't have
* git block git push to prevent the overwriting those remote updating
* before pushing you need to pull the changes from the remote local.
* git pull --rebase origin main
* git push origin main

