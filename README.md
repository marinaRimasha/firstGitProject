# README for the first repo created for IT Switcher school

**This file contains a brief description of the differences between a few git commands widely used for getting data from a repository**	

## Explanation of **`git pull`** and **`git fetch`** commands 

### Description
Both `git pull` and `git fetch` are Git commands used to retrieve changes from a remote repository to your local repository. However, they work differently and have distinct purposes. Here's a description and the main differences between `git pull` and `git fetch`:

1. **git pull**:
   - `git pull` is a combination of two operations: `git fetch` to fetch changes from the remote repository and `git merge` to merge those changes into your current branch.
   - By default, `git pull` fetches changes from the remote branch that is tracked by your current local branch (usually `origin/main` or `origin/master`).
   - If you want to fetch the latest changes from the remote repository and automatically merge them into your current branch, you can use `git pull`.

   See more details under [git pull documentation](https://git-scm.com/docs/git-pull) 

2. **git fetch**:
   - `git fetch` only performs the operation of fetching changes from the remote repository without automatically merging them into your current branch.
   - When you run `git fetch`, Git retrieves all changes from the remote repository but does not merge them into your local branch. Instead, it stores the fetched changes in separate "remote-tracking" branches (e.g., `origin/main` or `origin/master`), which you can review, compare, and manually merge later.
   - Use `git fetch` when you want to fetch the latest changes from the remote repository but are not yet ready to merge them into your local branch. This allows you to review changes and decide when and how to merge them.

   See more details under [git fetch documentation](https://git-scm.com/docs/git-fetch)

### Main Differences
- `git pull` performs `git fetch` and an automatic `git merge` with your current branch, while `git fetch` only fetches changes without automatic merging.
- `git pull` can result in merge conflicts if there are differences between your local branch and the remote branch, whereas `git fetch` only fetches changes without merging, thus avoiding merge conflicts.
- `git fetch` allows you to review fetched changes before merging, providing more control over the merging process.

![Image representation of differences between git pull and git fetch using visuals of comands and repository and local data.](https://s3.ap-south-1.amazonaws.com/s3.studytonight.com/tutorials/uploads/pictures/1622436019-103268.png )


_Both commands are essential when working with remote repositories in Git, and the choice between them depends on the specific situation and project requirements._