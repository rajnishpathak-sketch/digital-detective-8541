# Mission 3: Understanding the Operating System

## Objective

To understand how an operating system works, how it manages computer resources, and how to inspect system information and running processes using the macOS Terminal.

---

## Task 3.1: Exploring System Information

### Commands Used

```bash
sw_vers
uname -srm
whoami
df -h /
top -l 1 -n 10
```

### What I Learned

- `sw_vers` displays the macOS version and build information.
- `uname -srm` displays the operating system kernel name, kernel version, and machine architecture.
- `whoami` displays the username of the currently logged-in user.
- `df -h /` displays disk space usage in a human-readable format.
- `top -l 1 -n 10` displays a snapshot of system activity and running processes.

### Observations

- My system runs macOS on Apple Silicon architecture (`arm64`).
- The operating system is built on the Darwin kernel.
- The `df` command helped me understand total, used, and available disk space.
- The `top` command showed CPU usage, memory usage, and running processes.
- I learned that CPU usage changes depending on the applications and tasks running at that moment.

### Difficulties Faced

Initially, I was unsure about command flags such as `-l` and `-n`. I learned that flags are specific to each command and can have different meanings depending on the command being used.

---

## Task 3.2: Understanding Running Processes

### Commands Used

```bash
ps
ps aux
ps aux | head -n 6
pgrep -fl Safari
pgrep -fl "Visual Studio Code"
```

### What I Learned

- A process is an instance of a program that is currently running.
- Every process has a unique Process ID (PID).
- `ps` displays information about processes.
- `ps aux` provides a broader list of running processes.
- `head -n 6` displays the first six lines of command output.
- `pgrep -fl` searches for processes using a name or pattern.

### Observations

When I searched for Visual Studio Code, I found multiple related processes, including:

- Main application process
- GPU process
- Renderer processes
- Extension-related processes
- Language server processes

This helped me understand that modern applications can use multiple processes to handle different tasks independently.

### Difficulties Faced

I initially typed `pgrep -f1` instead of `pgrep -fl`. I learned that the lowercase letter `l` and the number `1` are different characters and that command syntax must be entered correctly.

---

## Task 3.3: Understanding Paths and File Permissions

### Commands and Concepts Explored

```bash
pwd
ls -l
chmod
chown
stat
```

### What I Learned

**1. Absolute and Relative Paths**

- An absolute path specifies the complete location of a file or directory, starting from the root directory (`/`).
- A relative path specifies a location in relation to the current working directory.

**2. File Permissions**

File permissions determine what actions users can perform on files and directories.

There are three basic permissions:

- `r` (Read): Allows reading file contents.
- `w` (Write): Allows modifying file contents.
- `x` (Execute): Allows executing a file or accessing a directory.

Permissions are assigned to three categories:

- Owner
- Group
- Others

**3. chmod**

The `chmod` command changes file or directory permissions.

Example:

```bash
chmod 755 filename
```

**4. chown**

The `chown` command changes the ownership of a file or directory.

Example:

```bash
sudo chown username filename
```

It can also change both the owner and group:

```bash
sudo chown username:groupname filename
```

**5. stat**

The `stat` command displays detailed information about a file, including its metadata.

### What I Understood

I learned that permissions control what users can do with files, whereas ownership identifies the user and group associated with those files.

I also understood that directory permissions affect access to the directory and its contents.

---

## Task 3.4: Understanding Operating System Responsibilities

An operating system acts as an intermediary between computer hardware, software, and the user.

Its major responsibilities include:

### 1. Process Management

- Manages running programs.
- Allocates CPU time to different processes.
- Handles process scheduling.
- Starts and terminates processes.

**Example:** macOS manages applications such as Safari and Visual Studio Code running simultaneously.

### 2. Memory Management

- Allocates RAM to applications.
- Tracks memory usage.
- Frees memory when it is no longer needed.
- Ensures efficient memory utilization.

**Example:** macOS manages memory usage between multiple open applications.

### 3. File Management

- Creates, deletes, and organizes files.
- Manages directories and storage.
- Controls file access and permissions.

**Example:** Finder allows users to browse and organize files on a Mac.

### 4. Device Management

- Manages connected hardware devices.
- Uses device drivers to communicate with hardware.
- Coordinates access to devices such as keyboards, printers, and speakers.

**Example:** macOS manages communication with the keyboard, speakers, and other connected devices.

### 5. Security and Access Control

- Manages user accounts and permissions.
- Protects system resources.
- Restricts unauthorized access.
- Controls application access to sensitive resources.

**Example:** macOS asks for permissions before applications can access the camera or microphone.

---

## Overall Learning

Through this mission, I learned how an operating system manages the computer's resources and coordinates different applications and hardware components.

I gained practical experience using Terminal commands to inspect system information, monitor processes, understand file permissions, and examine system activity.

I also understood the importance of process management, memory management, file management, device management, and security in the functioning of an operating system.

## Tools Used

- macOS
- Terminal
- Visual Studio Code

## Conclusion

This mission helped me understand the operating system beyond its graphical interface. I learned how to inspect my computer using Terminal commands and gained a better understanding of how macOS manages processes, memory, files, hardware, and security.