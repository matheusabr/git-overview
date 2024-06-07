## Tagging and Releases

Learn how to use tags and releases to improve the workflow of your git project. Here you have some explanations and examples of tagging and releasing in git.

### Contents

1.  [Types of Tags](#types-of-tags)
2.  [Create a Tag](#create-a-tag)
3.  [List Tags](#list-tags)
4.  [Checkout a Tag](#checkout-a-tag)
5.  [Delete a Tag](#delete-a-tag)
6.  [Release Workflow](#release-workflow)

---

### Types of Tags

You can choose the type of tag you want to create. There are some examples of how tags are commonly used in real-life git workflows:

1.  **Version Tags**: Tags are often used to mark specific versions of a project. For example, a project might use tags like `v1.0`, `v2.0`, `v2.1` to indicate different releases.
2.  **Release Tags**: Similar to version tags, release tags are used to mark specific points in a project's history that correspond to releases. For example, a project might use tags like `release-1.0`, `release-2.0` to mark official releases.
3.  **Hotfix Tags**: Tags can be used to mark hotfixes applied to a project's codebase. For example, a project might use tags like `hotfix-1.1.1` to mark a hotfix applied to version `1.1` of the project.
4.  **Feature Tags**: Tags can be used to mark the completion of a specific feature or functionality in a project. For example, a project might use tags like `feature-login`, `feature-payment` to mark the completion of these features.
5.  **Environment Tags**: Tags can be used to mark specific points in a project's history that correspond to different environments, such as `production`, `staging`, `development`.

These are just a few examples of how tags can be used in real-life Git workflows. The specific use cases and naming conventions for tags can vary depending on the project and team preferences.

### Create a Tag

Create a lightweight or annotated tag for a specific commit,

```shell
git tag <tag-name>                    # Lightweight tag
git tag -a <tag-name> -m "Tag message"   # Annotated tag
```

### List Tags

List all tags in the repository:

```shell
git tag
```

### Checkout a Tag

Checkout a specific tag to a new branch for inspection or to make changes:

```shell
git checkout -b <branch-name> <tag-name>
```

### Delete a Tag

Delete a tag from the repository:

```shell
git tag -d <tag-name>
```

### Release Workflow

A typical release workflow using tags:

1.  Create a new branch for the release:

    ```shell
    git checkout develop
    git checkout -b release-1.0
    ```

2.  Tag the release:

    ```shell
    git tag -a v1.0 -m "Version 1.0"
    ```

3.  Push the tag to the remote repository:

    ```shell
    git push origin v1.0
    ```

4.  Merge the release branch into the main branch:

    ```shell
    git checkout main
    git merge release-1.0
    ```

5.  Delete the release branch:

    ```shell
    git branch -d release-1.0
    ```
