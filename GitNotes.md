## Git Notes

- `git cherry-pick <commit>`  
  applies a specific commit from another branch into your current branch.

- `git stash`  
  Saves your uncommitted changes and cleans your working directory. Useful when switching branches without committing.

- `git stash apply`  
  Reapplies the latest stashed changes without removing them from the stash list.

- `git stash pop`  
  Reapplies the latest stash and removes it from the stash list.

- `git stash list`  
  Shows all stashed changes.

- `git stash drop <stash@{n}>`  
  Deletes a specific stash entry.

- `git stash clear`  
  Deletes all stash entries.