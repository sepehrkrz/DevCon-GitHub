# Branching and Merging Workflow Guide

## Activity Overview

This guide outlines the steps for a branching and merging workflow for a team. The activity involves creating a new branch, making changes, committing them, pushing to remote, merging branches, and handling merge conflicts.

---

### Step-by-Step Guide

#### For Everyone:

1. **Create a New Local Branch:**
   ```bash
   git checkout -b branch_name
2. **Publish the Branch to Remote:**
    ```bash
    git push --set-upstream origin branch_name
3. **Make a Small Change, Commit, and Push::**
Make your changes to the code.
Stage the changes
    ```bash
    git add .
    ```
    commit changes
    ```bash
    git commit -m "Your commit message"
    ```
    Push the changes to the remote repository
    ```bash
    git push
    ```
#### For All but One Team Member:
4. **Merge the Branch:**
    Ensure your local repository is up to date
    ```bash
    git pull
    ```
    Switch to the main branch:
    ```bash
    git checkout main
    ```
    Merge the branch_name branch into the main branch:
    ```bash
    git merge branch_name
    ```
    Push the merged changes to the remote repository:
    ```bash
    git push
    ```
5. **Checking for Merge Conflicts:**
    After merging, check for merge conflicts:
    ```bash
    git status
    ```
    Resolve any merge conflicts manually.
