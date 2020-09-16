---
title: "Git"
tags: ""
---

# Git

## Table of contents

-   [Git configs](#configuring-git)
-   [Getting Help](#help)
-   [Creating Snapshots](#creating-snapshots)
    -   [Initializing repo](#initializing-a-repository)
    -   [Staging](#staging-files)
    -   [Status](#viewing-status)
    -   [Commiting](#committing-staged-files)
    -   [Skipping staging](#skipping-staging-area)
    -   [Removing files](#removing-files)
    -   [Viewing Staged or Unstaged Changes](#viewing-staged-or-unstaged-changes)
    -   [Viewing History](#viewing-history)

## Configuring git

-   git config --global user.name "Kavin Valli"
-   git config --global user.email [kavinvalli@gmail.com](mailto:kavinvalli@gmail.com)
-   git config --global core.editor "code --wait"
-   git config --global -e (edit the configuration files as a file in vs code)
-   | Windows                           | Mac/Linux                      |
    | --------------------------------- | ------------------------------ |
    | git config --global core.autocrlf | git config --global core.input |

## Help

-   git config --help (fully extensive help)
-   git config  -h

## Creating Snapshots

### Initializing a repository

```sh
git init
```

### Staging files

```sh
git add file1.js          # Stages a single file
git add file1.js file2.js # Stages multiple files
git add *.js              # Stagres with a pattern
git add .                 # Stagres current directory and it's content
```

### Viewing Status

```sh
git status     # Long status
git status -s  # Short status
```

### Committing staged files

```sh
git commit -m "message" # Commits with one line message
git commit              # Opens a file where you can put in change description
```

### Skipping Staging area

```sh
git commit -am "message"
```
### Removing files

```sh
git rm file1.js  # Removes from working directory and staging area
git rm --cached file.js  # Removes only from staging area
```

### Viewing staged or unstaged changes

```sh
git diff              # Shows unstaged changes
git diff --staged     # Shows staged changes
```

### Viewing History

```sh
git log                # Full history
git log --oneline      # Sumary in one line for each commit
git log --reverse      # Lists the commit from oldest to newest
```