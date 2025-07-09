# Problem 3: Moving Multiple Commits Between Branches

## Task Description

A developer accidentally made multiple commits in the wrong branch and needs to move them to the correct one.

## What Was Done

- Created branch `feature` and made three changes in `change.txt`
- All changes (`line 1`, `line 2`, `line 3`) were committed in `feature`
- Realized the commits should be in `new-feature`
- Used `git cherry-pick` to move commits from `feature` to `new-feature`
- Reset `feature` branch back to match `master`

## Key Git Commands Used

```bash
git checkout -b feature
# changes and commits...
git checkout -b new-feature master
git cherry-pick <hash1> <hash2> ...
git reset --hard master  # on feature