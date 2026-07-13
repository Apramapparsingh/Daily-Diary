# Cyber Security Training - Day 5

**Date:** 07 July 2026

## Topics Covered

### 1. Important Linux System Files

Learned about important files stored in the `/etc` directory.

- `/etc/passwd` – Stores user account information.
- `/etc/shadow` – Stores encrypted user passwords (accessible only by the root user).
- `/etc/group` – Contains information about user groups.
- `/etc/gshadow` – Stores secure group password information.

### 2. User Management

Learned how to create and manage users in Linux.

**Commands practiced:**

```bash
sudo adduser user1
```

Set a password for the newly created user.

To view user details:

```bash
id user1
```

This command displays the User ID (UID), Group ID (GID), and the groups the user belongs to.

### 3. Group Management

Introduced to Linux groups and learned how users can be organized into groups for easier permission management.

### 4. Login Using Password

Learned how a user logs into the Linux system using a username and password, and how Linux verifies credentials using the password stored in `/etc/shadow`.

### 5. Introduction to Linux Directory Structure

Started learning the Linux directory structure and the purpose of important directories.

Also learned how to view the contents of system files using the `cat` command.

Example:

```bash
cat /etc/passwd
cat /etc/group
cat /etc/shadow
cat /etc/gshadow
```

## Commands Practiced

```bash
cat /etc/passwd
cat /etc/shadow
cat /etc/group
cat /etc/gshadow
sudo adduser user1
id user1
```

## Learning Outcome

By the end of Day 5, I understood the purpose of important Linux user and group files, learned how to create users, view user information, gained a basic understanding of group management, and began exploring the Linux directory structure.
