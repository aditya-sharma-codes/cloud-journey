# Day 1 – Linux Filesystem & Navigation

## Objective
Understand how the Linux filesystem works and how to navigate it confidently.
This is the foundation for working with cloud servers, virtual machines,
containers, and DevOps tools.

---

## 1. Core Linux Concepts

### Everything is a file
In Linux, everything is treated as a file:
- Files
- Directories
- Devices
- Configuration files

This design makes Linux simple and powerful.

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
|---------|--------|
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


ls
Lists visible files and directories.

```bash
ls