# Mission 2 – Become Comfortable with the Terminal

## 1. Mission Objective

The objective of this mission was to become comfortable using the Terminal to navigate directories, manage files, understand command flags and pipes, and learn about package managers.

## 2. Task 2.1 – Explore Basic Terminal Operations

I practised the following commands inside my assignment repository.

| Operation | Command | What it does | What I observed |
|---|---|---|---|
| Current-directory display | `pwd` | Displays the full path of the current working directory. | It displayed the path of my assignment repository. |
| Directory listing | `ls` | Lists files and folders in the current directory. | It displayed my mission folders and other files. |
| Detailed listing | `ls -l` | Displays files with permissions, ownership, size and modification date. | I could see additional information about each entry. |
| Change directory | `cd ..` | Moves to the parent directory. | My location changed to the parent folder. |
| Create directory | `mkdir terminal-practise` | Creates a new directory. | A practice folder was created. |
| Create empty file | `touch original.txt` | Creates an empty file. | The file appeared with a size of 0 bytes. |
| Copy file | `cp original.txt copy.txt` | Creates a copy of an existing file. | A separate copy was created. |
| Move / rename file | `mv copy.txt renamed-copy.txt` | Moves or renames a file. | The copied file was renamed. |
| Display file contents | `cat original.txt` | Displays the contents of a file. | The empty file displayed no text. |

## 3. Task 2.2 – Practise File Changes Safely

I created a text file named `notes.txt` and practised replacing and appending content.

### Commands used

```bash
touch notes.txt
echo "This is my first line." > notes.txt
echo "This is my second line." >> notes.txt
cat notes.txt
```

The output confirmed that both lines were present.

I then created a backup and renamed it:

```bash
cp notes.txt notes-backup.txt
mv notes-backup.txt final-backup.txt
cat final-backup.txt
```

### Answers to the written questions

**1. What is the difference between replacing a file's contents and adding text to the end?**

The `>` operator replaces the existing contents of a file, whereas `>>` appends new content to the end without removing the previous content.

**2. What is the difference between copying a file and moving a file?**

The `cp` command creates another copy while keeping the original file. The `mv` command moves a file to another location or renames it.

**3. What information does the current-directory display provide?**

The `pwd` command displays the full path of the directory in which I am currently working.

**4. Why is a directory-listing operation useful?**

The `ls` command helps us view files and folders in a directory. It is useful for locating files and checking the contents of a folder.

## 4. Task 2.3 – Understand Flags and Pipes

I practised normal and detailed directory listings.

```bash
ls
ls -lah
```

### Flags understood

| Flag | Purpose |
|---|---|
| `-l` | Displays a detailed listing. |
| `-a` | Includes hidden files and directories. |
| `-h` | Displays file sizes in a human-readable format. |

I observed that `ls -lah` displayed additional information such as permissions, file sizes, modification dates and hidden directory entries (`.` and `..`).

### Understanding pipes

A pipe (`|`) passes the output of one command as input to another command.

Commands practised:

```bash
ls -lah | head -n 3
ls -lah | tail -n 3
```

- `head -n 3` displays the first three lines.
- `tail -n 3` displays the last three lines.
- The pipe connects the commands and passes their output.

I understood that pipes allow multiple commands to work together without manually transferring their output.

## 5. Task 2.4 – Understand Package Managers

I explored Homebrew, a package manager commonly used on macOS.

### Commands used

```bash
brew --version
which brew
brew list
```

### Observations

- Homebrew version installed: 7.0.12
- Homebrew executable location: `/opt/homebrew/bin/brew`
- `brew list` displayed the installed formulae managed by Homebrew.

### Why are package managers useful?

A package manager helps users install, update and remove software. Homebrew simplifies software management on macOS through Terminal and also manages software dependencies. It allows users to maintain and inspect installed packages conveniently.

I checked my existing installation without installing or uninstalling anything.

## 6. What I Learned From This Mission

After completing this mission, I understood:

1. How to navigate directories using Terminal.
2. How to create, copy, move and rename files.
3. The difference between replacing and appending file contents.
4. How to inspect files and directories using listing commands.
5. How command flags change the behaviour of commands.
6. How pipes connect commands and filter their output.
7. The purpose of package managers and how Homebrew works.

## 7. Difficulties Faced and How I Resolved Them

Initially, I needed some practice understanding the difference between copying and renaming files. I also made a small typing mistake while renaming a file, which I corrected using the `mv` command.

Understanding the difference between `>` and `>>` was another important learning point. Practising both commands helped me understand how to preserve existing file contents while adding new text.

I also learned how flags and pipes can make Terminal commands more useful and informative.

## 8. Tools Used

- MacBook Pro
- macOS Terminal
- Homebrew
- Git and GitHub
- Visual Studio Code

