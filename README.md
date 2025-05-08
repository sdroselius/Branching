## Git Branching Practice

Git cheat sheet and branching practice.
Change made on main.

### Basic Commands
* `git init` - initialize local git repo in current folder (working directory)
* `git add .` - stage all changes for commit
* `git commit -m "message"` - commit staged changes to local repo

### Info Commands
* `git status` - show current status of working directory
* `git log` - show local commit history
* `git log --oneline` - show local commit history, compact format
* `git config -l` - list configuration of local repo
* `git config --global -l` - list global configuration
* `git version` - show version of installed git

### Branching Commands
* `git branch` - list local branches
* `git branch branchName` - create new branch `branchName`
* `git checkout branchName` - switch to branc `branchName`
* `git checkout -b branchName` - create and check out `branchName`

### Remote Commands
* `git remote add alias URL` - connect local repo to remote, using name `alias` for remote repo `URL`
* `git push alias branchName` - push local commits to remote repo `alias` on branch `branchName`

### Git Branch Workflow
1. Go to local `main` branch
   ```
   git checkout main
   ```
1. Pull remote main
   ```
   git pull origin main
   ```
1. Create and check out new branch
   ```
   git checkout -b featureName
   ```
1. Work on your branch, committing frequently
1. When task complete, pull main into your branch and fix merge conflicts
   ```
   git add .
   git commit -m "Complete feature"
   git pull origin main
   ```
   Fix any merge conflicts and commit the fix.
1. Push to your branch
   ```
   git push origin featureName
   ```
1. Create pull request on Github
1. Merge pull request to main









