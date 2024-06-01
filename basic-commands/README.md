## Git Basic Commands

This is your go-to guide for mastering the basic Git commands you need for everyday version control tasks. Let's dive in and make your Git journey fun and productive!

### Contents

1.  [Initialize a Repository](#initialize-a-repository)
2.  [Add Changes to the Staging Area](#add-changes-to-the-staging-area)
3.  [Commit Changes](#commit-changes)
4.  [Check Repository Status](#check-repository-status)
5.  [View Commit History](#view-commit-history)
6.  [Create and Switch Branches](#create-and-switch-branches)
7.  [Merge Branches](#merge-branches)

---

### Initialize a Repository

To start version controlling a new or existing project, you can initialize a Git repository in the project's root directory:

```shell
git init
```

### Add Changes to the Staging Area

Before committing changes, you need to add them to the staging area. You can add specific files or all changes:

```shell
git add <file>     # Add a specific file
git add .          # Add all changes
```

### Commit Changes

Commit your changes to the repository with a descriptive commit message:

```shell
git commit -m "Your commit message here"
```

### Check Repository Status

Check the status of your repository to see which files are modified, staged, or untracked:

```shell
git status
```

### View Commit History

View the commit history of your repository to see past commits and their messages:

```shell
git log
```

### Create and Switch Branches

Create a new branch and switch to it to work on new features or fixes:

```shell
git checkout -b <branch-name>   # Create and switch to a new branch
```

### Merge Branches

Merge changes from one branch into another (e.g., merge a feature branch into the main branch):

```shell
git checkout <branch-to-merge-into>
git merge <branch-to-merge>
```
