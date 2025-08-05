# Git Merge

# Why we use merge and branches:
We use them because problems can happen in structuring the project between team members in a company or a project. So, the owner is the only one who can access the main branch, which is the main part of the project. Everyone else has their own branches, and when they try to push, they need approval (or approvals) first.

# Commands we need
```
git checkout -b <name of branch> // Create and switch to a new branch
```
```
git checkout <name of branch>    // Switch to an existing branch
```
```
git push origin <branch-name>    // To push in the branch you want exactly
```

# Settings of repo (Gitea/Github)

1 - Access : Settings -> Branches -> Add New Rule
2 - Protected Branch Name Pattern : <name of the branch>
3 - Under Push -> Disable Puch (Turn On)
4 - Disable Force Push
5 - Pull Request Aprovale 0
6 - Under Pull Request Merge -> Enable Merge Allowlist add the ones who can approve
7 - Save