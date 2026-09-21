# Git Workflow Documentation

## Task 1: Add Overtime Pay

Added overtime pay calculation for shifts over 8 hours.

![Task 1 Screenshot](screenshots/task1.png)

---

## Task 2: Round Shift Pay

Changed the pay calculation to use rounding instead of truncating the result.

![Task 2 Screenshot](screenshots/task2.png)

---

## Task 3: Resolve Merge Conflict

Fetched the latest changes, merged the branches, resolved the conflict, and made sure all tests passed.

![Task 3 Screenshot](screenshots/task3.png)

---

## Task 4: Reconcile with Rebase

Rebased the local branch with the latest remote changes and updated the overtime test.

![Task 4 Screenshot A](screenshots/task4a.png)

![Task 4 Screenshot B](screenshots/task4b.png)

---

## Task 5: Merge Feature into Main

Merged the completed feature branch into main and verified that all tests passed.

![Task 5 Screenshot](screenshots/task5.png)

---

## Task 6: Finalize and Tag

Finalized the workflow, added the documentation and screenshots, and tagged the final synced version.

![Task 6 Screenshot](screenshots/task6.png)

---

# Questions/Reflections

### 1. What did the rejected push error message tell you, and why did it happen?

The rejected push error message said that the remote repository contained work that I did not have locally. This happened because changes had already been pushed from another clone, so my local branch was behind the remote branch.

### 2. What's the actual difference between how you resolved Task 3 (merge) vs Task 4 (rebase)?

In Task 3, I used `git fetch` and `git merge` to combine the changes from the remote branch with my local changes. This created a merge commit after I resolved the conflict. In Task 4, I used `git fetch` and `git rebase` to update my local branch by placing my local commit on top of the latest remote changes, keeping the commit history more linear.

### 3. What one habit would have avoided both rejected pushes in this lab?

The one habit that would have avoided both rejected pushes is checking or fetching the latest changes from the remote repository before pushing my changes.

### 4. Which approach - merge or rebase - would you default to on a shared team branch, and why?

I would default to merge on a shared team branch because it preserves the existing commit history and does not rewrite commits that other team members may already have. Rebase can be useful when working on my own feature branch and I want to keep the history cleaner.
