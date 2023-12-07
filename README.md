# Git Branching Cheat Sheet

## Basic Commands
* `git init` - initialize local git repository
* `git add .` - stage files in working directory for commit
* `git commit -m "msg"` - commit staged files with commit message `msg`

## Info Commands
* `git status` - show state of local working directory
* `git log` - list commit history
* `git log --oneline` - list commit history, compact format
* `git config -l` - list local git configuration
* `git help` - show synopsis of git commands

## Branching Commands
* `git branch` - list local branches
* `git branch branchName` - create local branch `branchName`
* `git checkout branchName` - move to branch `branchName`

## Remote Commands
* `git remote add origin URL` - set `origin` as alias for remote repo `URL`
* `git push origin branchName` - push local commits to `origin` repo on branch `branchName`

