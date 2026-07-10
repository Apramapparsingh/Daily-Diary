# Cyber Security Training - Day 3

**Date:** 03 July 2026

---

# Introduction

On the third day of my Cyber Security training, I learned about the Linux Directory Structure, which explains how files and directories are organized in the Linux operating system. I also studied Linux file permissions, file ownership, user privileges, password management, and system updates. These topics are fundamental for Linux system administration and cybersecurity.

---

# Linux Directory Structure

Linux follows a hierarchical directory structure that starts from the root directory (`/`). Every file and directory in the operating system is stored under the root directory.

## Common Linux Directories

| Directory | Description |
|-----------|-------------|
| `/` | Root directory of the Linux file system. |
| `/home` | Stores personal files and folders of normal users. |
| `/root` | Home directory of the root (administrator) user. |
| `/bin` | Contains essential user commands such as `ls`, `cp`, and `mv`. |
| `/sbin` | Contains system administration commands used by the root user. |
| `/etc` | Stores system configuration files. |
| `/usr` | Contains installed applications, libraries, and documentation. |
| `/var` | Stores variable data such as logs, cache, and mail files. |
| `/tmp` | Stores temporary files created by programs. |
| `/dev` | Contains device files representing hardware devices. |
| `/proc` | Virtual directory containing information about running processes and the Linux kernel. |
| `/boot` | Contains files required for booting the operating system. |
| `/opt` | Used to install optional third-party software packages. |

---

# Linux File Permissions

Linux uses three basic permissions to control access to files and directories.

| Permission | Symbol | Value | Description |
|------------|--------|-------|-------------|
| Read | `r` | 4 | Allows viewing the contents of a file. |
| Write | `w` | 2 | Allows modifying a file. |
| Execute | `x` | 1 | Allows executing a file or script. |

To check file permissions:

```bash
ls -l
```

---

# Changing File Permissions

The `chmod` command is used to modify file permissions.

Example:

```bash
chmod 110 hash.txt
```

Another example:

```bash
chmod 440 hash.txt
```

Symbolic method:

```bash
chmod u+rwx filename
```

Where:

- `u` = User (Owner)
- `g` = Group
- `o` = Others

---

# File Ownership

Every file in Linux has:

- Owner
- Group
- Others

To change the ownership of a file:

```bash
sudo chown root hash.txt
```

To verify ownership:

```bash
ls -l
```

---

# Root User and Normal User

Linux provides two types of users:

| User | Symbol |
|------|--------|
| Root User | `#` |
| Normal User | `$` |

The root user has complete administrative privileges, while a normal user has limited permissions.

---

# The `sudo` Command

The `sudo` command allows a normal user to execute commands with administrative (root) privileges.

Examples:

```bash
sudo chmod 440 hash.txt
```

```bash
sudo chown root hash.txt
```

---

# Changing the Root Password

To change the root password:

```bash
passwd root
```

If permission is denied:

```bash
sudo passwd root
```

---

# Updating the System

To update the package list in Kali Linux:

```bash
sudo apt update
```

Updating the system ensures that the latest package information and security updates are available.

---

# Commands Practiced

```bash
ls -l
chmod 110 hash.txt
chmod 440 hash.txt
chmod u+rwx filename
sudo chown root hash.txt
passwd root
sudo passwd root
sudo apt update
```

---

# Key Learning Outcomes

- Learned the Linux directory structure and the purpose of important system directories.
- Understood the role of the root directory (`/`) in Linux.
- Learned Linux file permissions (`r`, `w`, `x`) and their numeric values.
- Practiced changing file permissions using the `chmod` command.
- Learned about file ownership and the `chown` command.
- Understood the difference between the root user and a normal user.
- Learned the purpose and usage of the `sudo` command.
- Practiced changing the root password.
- Learned how to update Kali Linux using `sudo apt update`.

---

# Conclusion

Day 3 introduced the Linux directory structure and essential Linux administration concepts. I learned how Linux organizes its files and directories, how permissions and ownership help secure the system, and how administrative tasks are performed using the `sudo` command. These concepts provide a strong foundation for working with Kali Linux and are essential for cybersecurity professionals.
