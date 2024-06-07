## Advanced Features

There are some advanced Git features that can help you better manage your codebase and commit history. These features include rebasing, cherry-picking, stashing, interactive rebasing, and submodules.

### Contents

1. [Rebasing](#rebasing)
2. [Interactive Rebase](#interactive-rebase)
3. [Cherry-picking](#cherry-picking)
4. [Stashing](#stashing)
5. [Submodules](#submodules)

---

### Rebasing

Rebasing is used to reapply commits on top of another base commit. It can be used to maintain a linear commit history and integrate changes from one branch into another.

```shell
git rebase <base-branch>
```

In this example you'll going to rebase the `feature-b` branch onto the `develop` branch.

```shell
git checkout feature-b
git rebase develop
```

If you would like to abort a git rebase action, just use the abort option:

```shell
git rebase --abort
```

### Interactive Rebase

Interactive rebase allows you to interactively reapply commits from one branch onto another, giving you the opportunity to squash, edit, or reorder commits.

```shell
git rebase -i <base-branch>
```

### Cherry-picking

Cherry-picking allows you to pick a single commit from one branch and apply it to another branch.

```shell
git cherry-pick <commit-hash>
```

### Stashing

Stashing allows you to temporarily store changes that are not ready to be committed, so you can work on something else.

```shell
git stash
git stash apply
```

To list all stashed changes:

```shell
git stash list
```

To remove a stash, use the pop command:

```shell
git stash pop # Removes the last stash
git stash pop stash@{2} # Removes the stash with the given index
git stash drop stash@{2} # Removes the stash with the given index
git stash clear # Removes all stashes
```

### Submodules

Submodules allow you to include other repositories as subdirectories in your main repository.

```shell
git submodule add <repository-url>
```

To see the list of submodules:

```shell
git submodule status
```
