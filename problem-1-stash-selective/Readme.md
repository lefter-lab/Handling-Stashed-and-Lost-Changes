# Problem 1: Stashing and Selective Restore

## Task Description

A developer is working on multiple changes but wants to stash only specific modifications, not all.

## What Was Done

- Created a new branch `selective-stash`
- Modified two files: `featureA.txt` and `featureB.txt`
- Used `git stash push` to stash only changes in `featureA.txt`
- Confirmed that `featureB.txt` remained unchanged
- Switched to `master` and made unrelated changes
- Applied the stash without removing it from the stash list
- Verified that changes in `featureA.txt` were restored

## Key Git Commands Used

```bash
git stash push -m "Stash only A" featureA.txt
git stash list
git checkout master
git stash apply stash@{0}

