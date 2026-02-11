# Day 2 – Linux Permissions & Ownership

## Objective
Understand how Linux permissions work and how to control file access using chmod and chown.

---

## 1. Permission Structure

Each file has three permission categories:
- Owner
- Group
- Others

Each category can have:
- r (read)
- w (write)
- x (execute)

Example:
```bash
-rwxr-xr--
```


Breakdown:
- Owner → rwx
- Group → r-x
- Others → r--

---

## 2. Numeric Permission System

| Permission | Value |
|------------|-------|
| r | 4 |
| w | 2 |
| x | 1 |

Examples:
- 7 = rwx
- 6 = rw-
- 5 = r-x
- 4 = r--

Example:
```bash
chmod 755 file
```

Means:
Owner → 7 (rwx)
Group → 5 (r-x)
Others → 5 (r-x)

### 3. chmod Usage

Make file executable:
```bash
chmod +x file
```

Set specific permission:
```bash
chmod 700 file
```

### 4. chown Usage

Change owner:
```bash
sudo chown newowner file
```

### 5. Common Errors

Permission denied:
Happens when execute permission is missing.
Fix with chmod +x.

### Key Takeaways

Linux permissions control security.

chmod changes permissions.

chown changes ownership.

Numeric system (755, 700, etc.) is widely used in servers.

Essential for cloud environments.