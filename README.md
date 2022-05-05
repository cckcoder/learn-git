# First-Time Git Setup
view all of settings and where they are coming from using:
`git config --list --show-origin`

## Your Identity
The first thing should do when install git
set username and email
`git config --global user.name "codewizz"`
`git config --global user.email "codewizz@codewizz.com"`

## If want to override this with a different name or email for specific
when you in the project
`git config user.name "codewizz"`
`git config user.email "codewizz@codewizz.com"`

## Config editor
`git config --global core.editor "/usr/bin/vi"`

## Set default branch name
`git config --global init.defaultBranch main`

## Checking your settings
`git config --list`

## Git Help
* `git help`
* `git add -h`
* `git commit -h`

# Git Basics
* `git status`
* `git add <filename>`
    Example:
    * `git add README.md`

* git status short hand
    * `git status -s`

## Viewing your staged and Unstaged Change
* git diff `git diff`
    git diff use it most often to answer these two question
    * What have you changed but not yet staged?
    * What have you staged that you are about to commit?
    * Note! `git diff` by itself doesn't show all changes mad since
    your last commit only changes that are still unstaged.

* `git diff --staged`
    This command compares your staged changes to your last commit

## Commit
* you can commit and use favorite editor to write down the commit by
    * `git commit`
* Or short hand
    * `git commit -m "<commit message>"`

## Skipping staging area
If you want to skiping staging area, Git provide a simple shortcut
* `git commit -a -m "<commit message>"`

## Remove
* `git rm <filename>`

If you want to keep the file in working tree, but remove it from your staging
area. This is particularly useful if you forgot to add something to your
`.gitignore`

* `git rm --cached <filename>`
