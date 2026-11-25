# Mission 06: Git and GitHub

## 1. Mission Title
**Mission 06: Git and GitHub**

## 2. Task / Objective
The objective of this mission is to understand version control using Git and GitHub, learn basic Git commands, work with branches, create commits, and create a Pull Request without merging it.

## 3. Work Completed
- Learned the difference between Git and GitHub.
- Practised checking repository status and viewing commit history.
- Learned how to stage, commit and push changes.
- Created a new branch named `update-about`.
- Created an `about.txt` file containing my introduction and learning goals.
- Committed and pushed the file to GitHub.
- Created a Pull Request from `update-about` to `main`.
- Kept the Pull Request open without merging it.

## 4. Commands / Tools Used

**Commands used:**

| Command | Purpose |
|---|---|
| `git status` | Checks the current repository status. |
| `git add` | Stages changes for a commit. |
| `git commit -m "message"` | Saves staged changes. |
| `git push` | Uploads commits to GitHub. |
| `git pull` | Fetches and integrates remote changes. |
| `git log --oneline` | Displays commit history. |
| `git branch` | Lists available branches. |
| `git checkout -b update-about` | Creates and switches to a new branch. |
| `git remote -v` | Displays remote repository URLs. |

**Tools used:**
- macOS Terminal
- Git
- GitHub
- Visual Studio Code

## 5. My Understanding
Git is a version control system that tracks changes in files and helps developers manage project history.

GitHub is an online platform where Git repositories can be hosted and shared.

I learned that staging selects the changes for a commit, committing saves those changes locally, and pushing uploads commits to GitHub.

I also understood that branches allow developers to work on separate versions of a project without directly changing the main branch.

A Pull Request allows changes from one branch to be reviewed before they are merged into another branch.

## 6. Difficulties Faced
- Initially, I was confused about the difference between staging, committing and pushing.
- Understanding branches and switching between them took some practice.
- I was unsure about the purpose of the `-u` option in the push command.
- Understanding the base and compare branches while creating a Pull Request was challenging.

## 7. How I Resolved Them
- Practised Git commands and checked their outputs using `git status` and `git log`.
- Used `git checkout -b` to create and switch to a new branch.
- Learned that `-u` sets the upstream tracking branch.
- Explored the GitHub Pull Request page to understand the base and compare branches.
- Practised the Git workflow by making and pushing commits.

## 8. Evidence / Files
- `about.txt`
- `mission-06-git-github/README.md`
- `evidence/mission-06-git-github/pull-request.png`

The screenshot shows the Pull Request created for this mission.

## 9. Commit Details
- **Branch:** `update-about`
- **Commit message:** `Add about file`
- **Commit hash:** `383d3bb`
- **Pull Request:** [Add about file #1](https://github.com/rajnishpathak-sketch/digital-detective-8541/pull/1)
- **Base branch:** `main`
- **Compare branch:** `update-about`
- **Status:** Open and not merged

The Pull Request was intentionally kept open as required by the assignment.