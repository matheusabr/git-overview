## Git Workflows

There are many different Git workflows. This section will cover the most common workflows.

### Contents

1.  [Centralized Workflow](#centralized-workflow)
2.  [Feature Branch Workflow](#feature-branch-workflow)
3.  [Gitflow Workflow](#gitflow-workflow)
4.  [Forking Workflow](#forking-workflow)

---

### Centralized Workflow

The centralized workflow uses a central repository to collaborate. Developers clone the central repository, commit changes locally, and then push their changes to the central repository.

![Centralized Workflow](https://wac-cdn.atlassian.com/dam/jcr:0869c664-5bc1-4bf2-bef0-12f3814b3187/01.svg?cdnVersion=1794)

### Feature Branch Workflow

The feature branch workflow involves creating a new branch for each feature or bug fix. Developers work on their features in isolation and merge them back to the main branch when ready.

![Feature Branch Workflow](https://wac-cdn.atlassian.com/dam/jcr:09308632-38a3-4637-bba2-af2110629d56/07.svg?cdnVersion=1794)

### Gitflow Workflow

The Gitflow workflow defines a strict branching model designed around the project release. It uses branches like `develop`, `feature`, `release`, and `hotfix` to manage the project's lifecycle.

![Gitflow Workflow](https://wac-cdn.atlassian.com/dam/jcr:cc0b526e-adb7-4d45-874e-9bcea9898b4a/04%20Hotfix%20branches.svg?cdnVersion=1794)

### Forking Workflow

The forking workflow is commonly used in open-source projects. Contributors fork the main repository, clone their fork, make changes, push changes to their fork, and then create a pull request to merge changes back to the main repository.

![Forking Workflow](https://wac-cdn.atlassian.com/dam/jcr:0de71551-5c08-4fc4-ab6d-dc8a51bfcc5a/05.svg?cdnVersion=1794)

### References

Images and descriptions are from [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/comparing-workflows).
