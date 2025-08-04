
## Git Notes

```bash
git cherry-pick <commit>
```  
**`git cherry-pick`** applies a specific commit from another branch into your current branch.

```bash
git stash
```  
**`git stash`** saves your uncommitted changes and cleans your working directory. Useful when switching branches without committing.

```bash
git stash apply
```  
**`git stash apply`** reapplies the latest stashed changes without removing them from the stash list.

```bash
git stash pop
```  
**`git stash pop`** reapplies the latest stash and removes it from the stash list.

```bash
git stash list
```  
**`git stash list`** shows all stashed changes.

```bash
git stash drop <stash@{n}>
```  
**`git stash drop`** deletes a specific stash entry.

```bash
git stash clear
```  
**`git stash clear`** deletes all stash entries.