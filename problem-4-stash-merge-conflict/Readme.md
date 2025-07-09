## Problem 4: Stashing and Resolving Conflicts After Merge

### Task Description
A developer made local changes but had to temporarily stash them before pulling teammate's work, which results in a merge conflict when applying the stash.

### What Was Done
- Created a new file `conflict.txt` and added local content.
- Stashed the local changes using `git stash`.
- Simulated a teammate's change in the same file and committed it.
- Applied the stash, triggering a merge conflict in `conflict.txt`.
- Resolved the conflict manually by combining both changes.
- Finalized the resolution with a commit.

### Key Git Commands Used
- `git stash`
- `git add conflict.txt`
- `git commit -m "Add teammate change"`
- `git stash apply`
- Manual conflict resolution
- `git add conflict.txt`
- `git commit -m "Resolve merge conflict after stash apply"`
