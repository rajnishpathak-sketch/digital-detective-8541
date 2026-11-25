# Mission 6: Git and GitHub

## Objective

Learn how Git and GitHub work, understand the basic Git workflow, practise branching, create a Pull Request and become familiar with commonly used Git commands.

---

## Task 6.1: Understanding the Git Workflow

Git is a version control system that tracks changes in files and helps developers manage different versions of a project.

GitHub is an online platform that hosts Git repositories and allows developers to collaborate.

### Difference between Git and GitHub

- **Git:** Manages version history locally on a computer.
- **GitHub:** Hosts Git repositories online and supports collaboration.

### Basic Git workflow

| Operation | Command | Purpose |
|---|---|---|
| Check status | `git status` | Shows modified, staged and untracked files. |
| Stage changes | `git add filename` | Selects files for the next commit. |
| Create commit | `git commit -m "message"` | Saves staged changes in Git history. |
| Push changes | `git push` | Uploads commits to GitHub. |
| View history | `git log --oneline` | Displays previous commits. |

### Important concepts

- **Staging:** Selecting changes that should be included in the next commit.
- **Commit:** A saved snapshot of staged changes.
- **Push:** Uploading local commits to a remote repository.
- **Pull:** Fetching and integrating changes from a remote repository.

---

## Task 6.2: Working with Branches

A branch is an independent line of development that allows developers to work on changes without directly modifying the main branch.

### Commands used

Create and switch to a new branch:

```bash
git checkout -b update-about
```

Check available branches:

```bash
git branch
```

The `*` symbol indicates the currently active branch.

### Creating about.txt

Created a file named `about.txt` containing my introduction, education, current learning and career goal.

### Staging and committing

```bash
git add about.txt
git commit -m "Add about file"
```

### Pushing the branch to GitHub

```bash
git push -u origin update-about
```

The `-u` option sets the upstream tracking branch, making future pushes easier.

### Commit information

- Branch: `update-about`
- Commit message: `Add about file`
- Commit hash: `383d3bb`

---

## Task 6.3: Creating a Pull Request

A Pull Request (PR) is a request to merge changes from one branch into another. It allows developers to review changes before merging them.

### Steps followed

1. Opened my GitHub repository.
2. Navigated to the Pull Requests section.
3. Selected `update-about` as the compare branch.
4. Selected `main` as the base branch.
5. Added a title and description.
6. Created the Pull Request.

### Pull Request details

- **Title:** Add about file
- **PR Number:** #1
- **Base branch:** `main`
- **Compare branch:** `update-about`
- **Status:** Open
- **Merge conflicts:** None

### Pull Request link

[Add about file #1](https://github.com/rajnishpathak-sketch/digital-detective-8541/pull/1)

**Note:** I created the Pull Request but did not merge it, as the assignment required creating a PR without merging it.

---

## Task 6.4: Git Command Glossary

| Command | Explanation |
|---|---|
| `git init` | Initializes a new Git repository. |
| `git clone` | Copies a remote repository to the local computer. |
| `git status` | Displays the current repository status. |
| `git add` | Stages changes for a commit. |
| `git commit` | Saves staged changes in the repository history. |
| `git push` | Uploads local commits to a remote repository. |
| `git pull` | Fetches and integrates remote changes. |
| `git fetch` | Downloads remote updates without merging them. |
| `git branch` | Lists or creates branches. |
| `git switch` | Switches to another branch. |
| `git checkout -b` | Creates a new branch and switches to it. |
| `git merge` | Combines changes from another branch. |
| `git log` | Displays commit history. |
| `git diff` | Shows differences between file versions. |
| `git remote -v` | Displays configured remote repository URLs. |

---

## What I Learned

Through this mission, I learned:

1. How Git tracks changes and maintains project history.
2. The difference between Git and GitHub.
3. How staging, committing and pushing work.
4. How to create and switch between branches.
5. How branches allow developers to work independently.
6. How to create a Pull Request on GitHub.
7. Why code review is useful before merging changes.
8. Several commonly used Git commands.

## Difficulties Faced

- Initially, I was confused about the difference between staging, committing and pushing.
- I learned that creating a branch and switching to it are separate operations unless I use `git checkout -b` or `git switch -c`.
- I was initially confused about the purpose of the `-u` option in `git push`.
- I learned how the base and compare branches work while creating a Pull Request.

## Tools Used

- macOS Terminal
- Git
- GitHub
- Visual Studio Code

## Conclusion

This mission helped me understand the fundamentals of version control and collaboration using Git and GitHub. I practised creating branches, committing changes, pushing them to GitHub and creating a Pull Request.

I now have a better understanding of how developers manage project changes and collaborate on software projects.