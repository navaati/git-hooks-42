git-hooks-42
============

Git hooks, such as pre-commit, for 42 school dev environment

To install them in a git repo, copy them into the .git/hooks/ folder of your repo. Check that they have the execution rights.

At the moment the only hook available is a pre-commit hook.

## pre-commit

This hook check all .c source files with the norminette. If the norminette detects an error, the commit is cancelled.
It is thus impossible to commit a file with a norm error.

You can provide additionnal flags to the norminette in the NORM_EXTRA_FLAGS environment variable. Also if you set the NORM_WERROR variable (to wathever)
the hook will make the commit fail on norminette Warnings in addition to errors.
