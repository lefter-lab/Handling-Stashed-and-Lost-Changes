# Problem 2: Recovering Uncommitted Changes

## Task Description

A developer accidentally discards uncommitted changes and needs to recover them using Git.

## What Was Done

- Created and modified a file `critical.txt` with important content
- Discarded the uncommitted changes using `git reset` and `git checkout`
- Ran `git fsck --lost-found` to find the dangling blob
- Used `git show <blob>` to recover the lost content
- Restored the file and committed the recovered changes

## Key Git Commands Used

```bash
git add critical.txt
git reset
git checkout -- critical.txt
git fsck --lost-found
git show <blob_hash> > critical.txt
git add critical.txt
git commit -m "Recover lost changes in critical.txt"
