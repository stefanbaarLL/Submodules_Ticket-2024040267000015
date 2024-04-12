# Submodules_Ticket-2024040267000015
A few days ago I updated to Smartgit 23.1.2, and I just started a Chromium
bump, which involves rebasing a commit that deletes a number of submodules.

When these deleted submodules are updated upstream, a (command line) git
rebase triggers a merge conflict for these deleted submodules.

What I just discovered is that this "updated" Smartgit version does not
allow me to right-click these submodule and resolve the problem by Removing
the submodule, because the menu option was disabled, I had to use the
command line to remove the submodule.

Steps to reproduce (Stefan)
1. create repo wiht main and submodul https://github.com/stefanbaarLL/Submodules_Ticket-2024040267000015
2. create feautre branch and delete submodule
3. change submodul in remote
4. I expect a conflict
