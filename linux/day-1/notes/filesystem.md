# Day 1 – Linux Filesystem & Navigation

## Objective
Understand how the Linux filesystem works and how to navigate it confidently.
This is the foundation for working with Linux servers, cloud VMs, containers,
and DevOps tools.

---

## 1. Core Linux Concepts

### Everything is a file
In Linux, everything is treated as a file:
- Files
- Directories
- Devices
- Configuration files

Everything is treated as a file.

---

### Case Sensitivity
Linux is case-sensitive:
- `Cloud`
- `cloud`
- `CLOUD`

All are different.

---

## 2. Important Directories (Cloud-Relevant)

| Directory | Purpose |
|----------|---------|
| `/` | Root of the filesystem |
| `/home` | User home directories |
| `/home/aditya` | My home directory |
| `/etc` | System configuration files |
| `/var` | Logs and runtime data |
| `/usr` | Installed programs |
| `/tmp` | Temporary files |

Cloud servers follow the same structure.

---

## 3. Basic Commands Learned

### pwd
Prints the current working directory.

```bash
pwd
```


list :-

### ls – List Files
Lists visible files and directories.

```bash
ls
```
Displays detailed information.
```bash
ls -l
```

Example output:
drwxr-xr-x 3 aditya aditya 4096 Feb 9 23:12 cloud-journey

Permission breakdown:

d → directory
rwx → owner permissions
r-x → group permissions
r-x → others permission
aditya → owner and group
ls -a – Show Hidden Files
Displays all files including hidden ones.
ls -a
Hidden files start with a dot (.).

### 4. Hidden Files

Hidden files store configuration and system settings.
Examples:
.bashrc → shell configuration
.gitconfig → Git global configuration
.ssh → SSH keys and known hosts

To view hidden files:
```bash
ls -a
```
### 5. Directory Navigation

cd – Change Directory
Relative path
cd cloud-journey

Absolute path
cd /home/aditya/cloud-journey
```bash
cd ..
```
Moves to the parent directory.
```bash
cd ~
```
Moves to the home directory.

For this system:
~ = /home/aditya

### 6. Special Symbols in Linux
Symbol	Meaning
.	Current directory
..	Parent directory
~	Home directory
/	Root directory

### 7. Creating Files and Directories

Create a directory
```bash
mkdir directory_name
```
Create a file
```bash
touch file_name
```
Example:
```bash
mkdir notes
touch notes/filesystem.md
```
### 8. Viewing File Structure
tree Command

Displays directory structure visually.
```bash
tree ~/cloud-journey
```
This helps understand project layouts clearly.


### 9. Errors Encountered and Their Meaning
"Not a directory"
Occurs when trying to use cd on a file.
Example:
```bash
cd filesystem.md
```
Reason:
cd works only with directories, not files.

"Permission denied"

Occurs when trying to execute a non-executable file.
Example:
./filesystem.md

Reason:
The file does not have execute permission
.md files are meant to be opened, not executed

### 10. Git Usage (Day 1)

Commands used:
git status
git add .
git commit -m "Day 1: Linux filesystem and navigation basics"
git push


Purpose:

Track learning progress
Build consistency
Maintain a public learning log on GitHub

Key Takeaways :- 

Linux filesystem is structured and predictable
cd works only with directories
Hidden files store important configurations
Absolute and relative paths behave differently
This knowledge directly applies to:
Cloud virtual machines
Linux servers
Docker containers
Production environments



---

