## Branching and Merging

There's some explanations and examples of creating new branches, switching between branches, merging branches, resolving merge conflicts, and deleting branches.

### Contents

1.  [Create a New Branch](#create-a-new-branch)
2.  [Switch Branches](#switch-branches)
3.  [Merge Branches](#merge-branches)
4.  [Resolve Merge Conflicts](#resolve-merge-conflicts)
5.  [Delete a Branch](#delete-a-branch)

---

### Create a New Branch

Create a new branch to work on a new feature or fix based on the current branch (e.g. develop) :

```shell
git checkout develop
git checkout -b <branch-name>
git checkout -b feature/authentication # For example
```

### Switch Branches

Switch between branches in your repository:

```shell
git checkout develop
git checkout <branch-name>
git checkout feature/authentication # For example
```

### Merge Branches

Merge changes from one branch into another:

1. Checkout to the target branch (e.g. develop)

```shell
git checkout develop
```

2. Merge the changes from one branch into the target branch

```shell
git merge <branch-name>
git merge feature/authentication # For example
```

### Resolve Merge Conflicts

If there are conflicts during a merge, resolve them manually:

1.  Open the conflicting file(s) in your code editor.
2.  Locate and resolve the conflicts.
3.  Add the resolved files to the staging area:

    ```shell
    git add <resolved-file> # Add each resolved file to the staging area
    git add . # or add all resolved files
    ```

4.  Commit the merge:

    ```shell
    git commit -m "Merge branch 'branch-name' into <develop>"
    git commit -m "Merge branch 'feature/authentication' into <develop>" # For example
    ```

### Delete a Branch

Delete a branch locally after it has been merged (optional) or is no longer needed:

```shell
git branch -d <branch-name> # It deletes locally
git branch -d feature/authentication # For example
```

To delete a remote branch you need to specify the remote location and the branch name.

```shell
git push <remote> --delete <branch>
git push origin --delete feature/authentication # For example
```

> **Note**: after delete any remote branch, it is important to run `git fetch --all --prune` to remove all obsolete local remote-tracking branches for any remote branches that no longer exist on the remote.
