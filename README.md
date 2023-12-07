# Git Branching Cheat Sheet

## Overview

Summary of common git commands, and practice with branching.

## Summary of Branch Workflow

1. Checkout and pull main
   ```bash
   git checkout main
   git pull origin main
   ```
1. Checkout new branch from up-to-date main
   ```bash
   git checkout -b someFeature
   ```
1. Work, committing each completed task, until feature is complete
1. Pull remote main into local branch
   ```bash
   git add .
   git commit -m "Complete feature"
   git pull origin main
   ```
   * If auto merge succeeds, save and quit from `vi` editor:
     ```
     :wq
     ```
   * If `CONFLICT`, fix conflicts in all files removing merge markers and commit
     ```bash
     git add .
     git commit -m "Fix merge conflicts"
     ```
1. Push to remote branch
   ```bash
   git push origin someFeature
   ```
1. On Github, create pull request and merge with main
1. Checkout and pull merged main
   ```bash
   git checkout main
   git pull origin main
   ```

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
* `git checkout -b branchName` - create and move to `branchName`

## Remote Commands
* `git remote add origin URL` - set `origin` as alias for remote repo `URL`
* `git push origin branchName` - push local commits to `origin` repo on branch `branchName`
* `git pull origin branchName` - pull remote branch `branchName` into current local branch

