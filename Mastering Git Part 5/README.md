## MASTERING GIT:
# ** Part 5: Merging Two Branches in GitHub: A Step-by-Step Guide

![Alt text](<images/Mastering git 5.drawio.png>)

Merging branches in GitHub is a fundamental operation in version control that allows developers to combine changes from one branch into another. Whether you're working on a feature branch, fixing a bug, or managing a long-term development branch, understanding how to merge branches is crucial. In this guide, I'll walk you through the steps of merging two branches in GitHub, complete with explanations and commands.

## Prerequisites

Before we begin, make sure you have the following:

- A GitHub account
- A repository with at least two branches
- Git installed on your local machine
- Basic knowledge of Git and GitHub

## Step 1: Clone the Repository

Start by cloning the repository to your local machine if you haven't already. Replace `<repository_url>` with the actual URL of your GitHub repository.

```bash
git clone <repository_url>
cd <repository_directory>
```

## Step 2: Check Current Branch

Ensure you are on the branch where you want to merge changes into. You can list all local branches and check the current branch with:

```bash
git branch
```

To switch to a different branch, use:

```bash
git checkout <branch_name>
```

## Step 3: Update the Current Branch

It's essential to have the latest changes from the target branch (the one you want to merge into). Fetch the latest updates from the remote repository:

```bash
git fetch origin
```

## Step 4: Merge the Target Branch

Now, you are ready to merge the target branch into your current branch. Use the `git merge` command:

```bash
git merge <target_branch>
```

For example, if you want to merge the `feature/new-feature` branch into the current branch:

```bash
git merge feature/new-feature
```

## Step 5: Resolve Conflicts (If Any)

If there are conflicting changes between the branches you're merging, Git will prompt you to resolve them. Open the conflicted files, resolve the conflicts, and save the changes.

After resolving conflicts, add the modified files to the staging area and continue the merge:

```bash
git add <conflicted_files>
git commit
```

## Step 6: Push Changes to GitHub

Once the merge is complete and there are no conflicts or after you've resolved them, push the changes to GitHub:

```bash
git push origin <current_branch>
```

## Step 7: Confirm the Merge on GitHub

Go to your GitHub repository in a web browser and navigate to the "Pull Requests" tab. You should see your recently pushed branch with a message indicating that you pushed new changes.

Click the "Compare & pull request" button.

## Step 8: Create a Pull Request

In the pull request interface, you can review the changes. Provide a title and description for your pull request to explain the purpose of the merge.

Click the "Create pull request" button.

## Step 9: Review and Merge

Now, the pull request is created, and team members can review the changes. Once approved, click the "Merge pull request" button.

## Step 10: Confirm the Merge

GitHub will ask you to confirm the merge. You can choose to delete the source branch after merging if it's no longer needed.

Click the "Confirm merge" button.

Congratulations! You've successfully merged two branches in GitHub.

Merging branches is a fundamental aspect of collaboration and version control. By following these steps, you can efficiently integrate changes from one branch into another, ensuring your project stays organized and up-to-date.

Happy coding! 🚀 #GitHub #Git #VersionControl #Development #OpenSource