All commands and workflow tips learnt:

git commit --amend (This replaces the last commit with a new one you edit. Only do this on commits that have not been pushed anywhere, and notify anyone you're working with.)

git rebase -i --root orgit  HEAD~{Amount of commits to go back} (This will allow you to make changes to multiple commits at the same time. Notify anyone you're working with, as ths is dangerous.)

squash (Important when rebasing to merge commits together. This cleans our git history and makes commits more manageable to read.)

git push --force (Rewrites the remote repository with your own local history. Very dangerous when working with others, as it can delete whatever no one else but you has.)

git push --force-with-lease (A more fail-safe version)

git revert HEAD (This will allow you to revert the changes you pushed)

git config --global core.editor "code --wait" (This allows you to use your text editor instead of VIM when writing commit messages.)

Best practices (In most cases):

Don't push after every single commit, changing published history should be avoided.

Never amend commits that have been pushed

Never rebase a repository multiple people work on

Never reset commits that have been pushed