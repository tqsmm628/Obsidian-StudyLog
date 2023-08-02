---
subtitle: A Hands-On and Visual Guide to the Basics of Git
source: google play
publisher: o'reilly
author: Anna Skoulikari
status: doing
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

