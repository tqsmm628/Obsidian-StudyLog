---
subtitle: A Hands-On and Visual Guide to the Basics of Git
publisher: o'reilly
author: Anna Skoulikari
status: done
---
#book

# Preface

# 1. Git and the Command Line

## What Is Git?

==Example Book Project 1-1

## The Graphical User Interface and the Command Line

## Opening a Command Line Window

==FIGURE 1-1 An example of a command prompt

## Executing Commands in the Command Line

==FIGURE 1-2 How to execute a command included in a Follow Along section

### COMMAND OUTPUT

### EXECUTING THE FIRST COMMAND IN THE COMMAND LINE

```bash
git version
```

## Installing Git

## Command Options and Arguments

==FIGURE 1-3 An example of a command with an option and an argument

## Clearing the Command Line

```bash
clear
```

## Opening the Filesystem Window

## Working with Directories

```bash
pwd
```

### VIEWING THE CONTENTS OF DIRECTORIES

```bash
ls
ls -a
```

### NAVIGATING INTO AND OUT OF A DIRECTORY

```bash
cd desktop
pwd
```

```bash
cd ..
pwd
```

### CREATING A DIRECTORY

```bash
mkdir <directory_name>
```

```bash
cd desktop
mkdir rainbow
ls
```

```bash
cd rainbow
pwd
```

## Closing the Command Line

```bash
pwd
# close and reopen
#---------------------
pwd
cd desktop
pwd
```

## Setting Git Configurations

```bash
git config --global --list
```

```bash
git config --global user.name "<name>"
git config --global user.email "<email>"
```

```bash
git config --global user.name "1010496"
git config --global user.email "1010496@iisigroup.com"
git config --global --list
```

## Preparing a Text Editor

## Integrated Terminals

## Summary

# 2. Local Repositories

## Current Setup

## Introducing Repositories

## Initializing a Local Repository

```bash
git init
git init -b <branch_name>
```

## The Areas of Git

### Introducing the Working Directory

### Introducing the Staging Area

### What is a Commit?

### Introducing the Commit History

## Adding a File to a Git Project

## Summary

# 3. Making a Commit

## Current Setup

## Why Do We Make Commits?



## The Two Steps to Make a Commit

```bash
git status
```

### Adding Files to the Staging Area

```bash
git add <filename>
git add <filename> <filename>
git add -A
```

```bash
git add rainbowcolors.txt
git status
```

### Making a Commit

```bash
git commit -m 'red'
```

## Viewing a List of Commits

```bash
git log
```

## Summary

# 4. Branches

## State of the Local Repository

## Why Do We Use Branches?

### What Exactly are Branches in Git?

```bash
git log
```

### A bit of Git History: Master and Main

## Unmodified and Modified Files

```bash
git status
echo "Orange is the second color of the rainbow" >> rainbowcolors.txt
git status
```

```bash
git add rainbowcolors.txt
git status
```

## Making Commits on a Branch

```bash
git commit -m "orange"
git log
```

```bash
git cat-file -p $(git rev-parse --short HEAD)
```

## Creating a Branch

```bash
git branch
git branch <new_branch_name>
```

```bash
git branch
git branch feature
git log
```

## What Is HEAD?

## Switching Branches

```bash
git switch <branch_name>
git checkout <branch_name>
```

```bash
git branch
git switch feature
git branch
git log
```

## Working on a Separate Branch

```bash
echo "Yellow is the third color of the rainbow." >> rainbowcolors.txt
git add rainbowcolors.txt
git commit -m "yellow"
git log
```

## Summary

# 5. Merging

## State of the Local Repository

## Introducing Merging

## Types of Merges

- Fast-forward merges
- Three-way merges

## Doing a Fast-Forward Merge

```bash
git merge <branch_name>
```

### Switching onto the Branch you are Merging into

#### Git protects you from losing uncommitted changes

```bash
git status
echo "Green is the fourth color of the rainbow." >> rainbowcolors.txt
git status
git switch main
```

#### Switching branches changes files in the working directory

```bash
git switch main
git log
```

#### Viewing a list of all commits

```bash
git log --all
```

### Using the Git Merge Command to Execute a Merge

```bash
git merge feature
git log
```

## Checking Out Commits

```bash
git checkout <commit_hash>
```

```bash
git checkout 91f9043
git log --all
```

```bash
git switch main
git log
```

## Creating a Branch and Switching onto It in One Go

```bash
git switch -c <new_branch_name>
git checkout -b <new_branch_name>
```

## Summary

# 6. Hosting Services and Authentication

## Hosting Services and Remote Repositories

## Setting Up a Hosting Service Account

## Setting Up Authentication Credentials

### Using HTTPS

### Using SSH

## Summary

# 7. Creating and Pushing to a Remote Repository

## State of the Local Repository

## The Two Ways to Start Work on a Git Project

### Starting from a Local Repository

```bash
git push
```

### Starting from a Remote Repository

## The Interaction Between Local and Remote Repositories

## Why Do We Use Remote Repositories?

## Creating a Remote Repository with Data

### Creating the Remote Repository

### Adding a Connection to the Remote Repository

```bash
git remote add <shortname> <URL>
```

```bash
git remote
git remote -v
```

```bash
git remote
git remote add origin https://github.com/gitlearningjourney/rainbow-remote.git
git remote
git remote -v
```

### Introducing Remote Branches and Remote-Tracking Branches

### Pushing to a Remote Repository

```bash
git push <shortname> <branch_name>
```

```bash
git branch --all
```

```bash
git push origin main
git branch --all
git log
```

```bash
git switch feature
git push origin feature
git branch --all
git log
```

## Working on a Remote Repository Directly on a Hosting Service

## Summary

# 8. Cloning and Fetching

## State of the Local and Remote Repositories

## Cloning a Remote Repository

### The Collaboration Simulation

```bash
git clone <URL> <directory_name>
```

```bash
git clone https://github.com/gitlearningjourney/rainbow-remote.git friend-rainbow
```

```bash
cd friend-rainbow
git remote -v
git branch --all
git log
```

### What is origin/HEAD?

### Cloning Repositories and Different Types of Branches

```bash
git branch --all
git switch feature
git branch --all
```

### The origin Shortname

## Deleting Branches

```bash
git push <shortname> -d <branch_name>
```

```bash
git branch -d <branch_name>
```

```bash
git branch --all
git push origin -d feature
git branch --all
git switch main
git branch -d feature
git branch --all
```

## Git Collaboration and Branches

### Making a Commit in the Local Repository

```bash
echo "Green is the fourth color of the rainbow." >> rainbowcolors.txt
git add rainbowcolors.txt
git commit -m "green"
git log
```

### Pushing to the Remote Repository

```bash
git branch -vv
```

```bash
git branch -vv
git status
```

```bash
git push
git status
git log
```

## Incorporating Changes from the Remote Repository

### Fetching Changes form the Remote Repository

```bash
git fetch <shortname>
git fetch
```

```bash
git log --all
git fetch
git log --all
```

### Integrating Changes into a Local Branch

```bash
git switch main
git merge origin/main
git log
```

## Deleting Branches (Continued)

```bash
git fetch -p
```

```bash
git branch --all
git fetch -p
git branch --all
git branch -d feature
git branch --all
```

# 9. Three-Way Merges

## State of the Local and Remote Repositories

## Why Are Three-Way Merges Important?

## Setting Up a Three-Way Merge Scenario

```bash
echo 'Brown is not a color in the rainbow.' > othercolors.txt
git add othercolors.txt
git commit -m 'brown'
git log
```

## Defining Upstream Branches

```bash
git branch -u <shortname>/<branch_name>
```

```bash
git branch -vv
git branch -u origin/main
git branch -vv
```
## Editing the Same File Multiple Times Between Commits

```bash
git status
```

```bash
echo 'Bloo is the fifth color of the rainbow.' >> rainbowcolors.txt
git status
```

```bash
git add rainbowcolors.txt
git status
```

```bash
# fix typo
git status
```

```bash
git add rainbowcolors.txt
git status
```

## Working at that Same Time as Others on Different Files

```bash
git commit -m 'blue'
git push
git log
```

## Three-Way Merge in Practice

### Introducing VIM, the Command Line Text Editor

### Executing the Three-Way Merge

```bash
git fetch
git merge origin/main
# edit commit message
git log
```

```bash
git cat-files -p 2258399
git push
git log
```

## Pulling Changes from a Remote Repository

```bash
git pull <shortname> <branch_name>
git pull
```

```bash
git pull
git log
```

## State of the Local and Remote Repositories

## Summary

# 10. Merge Conflicts

## State of the Local and Remote Repositories

## Introducing Merge Conflicts

## How to Resolve Merge Conflicts

## Setting Up a Merge Conflict Scenario

```bash
echo 'Indigo is the sixth color of the rainbow.' >> rainbowcolors.txt
git add rainbowcolors.txt
git commit -m 'indigo'
git push
git log
```

```bash
echo 'Violet is the seventh color of the rainbow.' >> rainbowcolors.txt
git add rainbowcolors.txt
git commit -m 'violet'
git log
```

```bash
git fetch
git status
git log --all
```

## The Merge Conflict Resolution Process

### Step 1

### Step 2

### Aborting a Merge

```bash
git merge --abort
```

## Resolving Merge Conflicts in Practice

```bash
git merge origin/main
git status
# fix merge conflicts
# remove markers
git add rainbowcolors.txt
git status
git commit -m 'merge commit 2'
git log
```

## Staying Up to Date with a Remote Repository

## Syncing the Repositories

```bash
git push
git log
git pull
git log
```

## State of the Local and Remote Repositories

## Summary

# 11. Rebasing

## State of the Local and Remote Repositories

## Integrating Changes in Git

```bash
git reabase <branch_name>
```

## Why Is Rebasing Helpful?

## Setting Up the Rebasing Example

```bash
echo 'Gray is not a color in the rainbow.' >> othercolors.txt
git add othercolors.txt
git commit -m 'gray'
git push
git log
```

## Unstaging and Staging Files

```bash
echo 'Black is not a color in the rainbow.' >> othercolors.txt
echo 'These are the colors of the rainbow.' >> rainbowcolors.txt
git status
```

```bash
git add rainbowcolors.txt othercolors.txt
git status
```

```bash
git restore --staged <filename>
```

```bash
git restore --staged rainbowcolors.txt
git status
```

```bash
git commit -m 'black'
git status
git log
```

```bash
git add rainbowcolors.txt
git commit -m 'rainbow'
git log
```

## Preparing to Rebase

```bash
git fetch
git log --all
```

## The Five Stages of the Rebase Process

### Stage 1: Find the Common Ancestor

### Stage 2: Store Information about the Branches involved in the Rebase

### Stage 3: Reset HEAD

### Stage 4: Apply and Commit the Changes

### Stage 5: Switch onto the Rebased Branch

## Rebasing and Merge Conflicts

```bash
git rebase --continue
git rebase --abort
```

## Rebasing a Branch in Practice

```bash
git rebase origin/main
git status
```

```bash
git add othercolors.txt
git status
git rebase --continue
git log
```

## The Golden Rule of Rebasing

## Syncing the Repositories

```bash
git push
git log
git pull
git log
```

## State of the Local and Remote Repositories

## Summary

# 12. Pull Requests (Merge Requests)

## State of the Local and Remote Repositories

## Introducing Pull Requests

## Hosting Service Specifics

## Why Use Pull Requests?

## Understanding How Pull Requests Are Merged

## Preparing to Make a Pull Request

```bash
git switch -c topic
echo 'Pink is not a color in the rainbow.' >> othercolors.txt
git add othercolors.txt
git commit -m 'pink'
git log
```

## An Easier Way to Define Upstream Branches

```bash
git branch -vv
git push
git push --set-upstream origin topic
git branch -vv
git log
```

## Creating a Pull Request on a Hosting Service

## Reviewing and Approving a Pull Request

## Merging a Pull Request

## Deleting Remote Branches

## Syncing the Local Repositories and Cleaning Up

```bash
git switch main
git pull -p
git branch -d topic
git log
```

```bash
git pull
git log
```

## State of the Local and Remote Repositories

## Summary

# Epilogue

# Appendix A. Chapter Prerequisites

## Prerequisite Setup for All Chapters

```bash
git config --global user.name '<name>'
git config --global user.email '<email>'
```

## Chapter 2 Prerequisite Setup

```bash
cd desktop
mkdir rainbow
cd rainbow
```

## Chapter 3 Prerequisite Setup

```bash
git init -b main
echo 'Red is the first color of the rainbow.' > rainbowcolors.txt
```

## Chapter 4 Prerequisite Setup

```bash
git add rainbowcolors.txt
git commit -m 'red'
```

## Chapter 5 Prerequisite Setup

```bash

echo 'Orange is the second color of the rainbow.' >> rainbowcolors.txt
git add rainbowcolors.txt
git commit -m 'orange'
git branch feature
git switch feature
echo 'Yellow is the third color of the rainbow.' >> rainbowcolors.txt
git add rainbowcolors.txt
git commit -m 'yellow'
```

## Chapter 6 and 7 Prerequisite Setup

```bash

git switch main
git merge feature
```

## Chapter 8 Prerequisite Setup

```bash
git switch feature
git push origin feature
```

## Chapter 9 Prerequisite Setup

```bash
git remote add origin
git push origin main
git clone ... friend-rainbow
cd friend-rainbow
```

## Chapter 10 Prerequisite Setup

## Chapter 11 Prerequisite Setup

## Chapter 12 Prerequisite Setup

# Appendix B. Command Quick Reference

## Chapter 1

```bash
clear
pwd
ls
ls -a
cd <path_to_directory>
mkdir <directory_name>
git config --global --list
git config --global user.name '<name>'
git config --global user.email '<email>'
```

## Chapter 2

```bash
git init
git init -b <branch_name>
```

## Chapter 3

```bash
git status
git add <filename>
git add <filename> <filename>
git add -A
git commit -m '<message>'
git log
```

## Chapter 4

```bash
git branch
git branch <new_branch_name>
git switch <branch_name>
git checkout <branch_name>
```

## Chapter 5

```bash
git merge <branch_name>
git log --all
git checkout <commit_hash>
git switch -c <new_branch_name>
git checkout -b <new_branch_name>
```

## Chapter 7

```bash
git push
git remote add <shortname> <URL>
git remote
git remote -v
git push <shortname> <branch_name>
git branch --all
```

## Chapter 8

```bash
git clone <URL> <directory_name>
git push <shortname> -d <branch_name>
git branch -d <branch_name>
git branch -vv
git fetch <shortname>
git fetch
git fetch -p
```

## Chapter 9

```bash
git branch -u <shortname>/<branch_name>
git pull <shortname> <branch_name>
git pull
```

## Chapter 10

```bash
git merge --abort
```

## Chapter 11

```bash
git rebase <branch_name>
git restore --staged <filename>
git rebase --continue
git rebase --abort
```

# Appendix C. Visual Language Reference

## Commits

## Git Diagram

## Repository Diagram