# Git Workflow Reflection

## 1. What did the rejected push error say and why?

The rejected push error said that the remote repository contained work that I did not have locally. This happened because changes were pushed from another clone of the same repository, so my local branch was behind the remote branch. Git rejected the push to prevent the remote changes from being overwritten.

## 2. What is the difference between the merge resolution in Task 3 and the rebase resolution in Task 4?

In Task 3, I used `git fetch` and `git merge` to combine the changes from the remote branch with my local changes. This created a merge history after resolving the conflict.

In Task 4, I used `git fetch` and `git rebase` instead. Rebase placed my local commit on top of the updated remote branch, which kept the history more linear.

## 3. What one habit would have avoided both rejected pushes?

One habit that could have avoided both rejected pushes is checking or fetching the latest remote changes before starting new work. This helps make sure the local branch is updated before making and pushing new changes.

## 4. Which approach, merge or rebase, would you default to on a shared team branch, and why?

I would default to merge on a shared team branch because it keeps the existing commit history and does not rewrite commits that other team members may already have. Rebase can also be useful when working on a personal feature branch and a cleaner history is needed.
