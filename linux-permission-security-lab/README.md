# Linux Permissions & Security Basics Lab

## Objective

Understand how Linux permissions, ownership, users, and access control work while practicing real troubleshooting scenarios related to file access and security.

---

# Technologies Used

- AlmaLinux
- Linux Permissions
- VirtualBox

---

# What I Learned

- Linux file permissions
- Ownership and groups
- chmod usage
- chown usage
- User management
- Linux access control
- Troubleshooting permission errors
- Multi-user environments

---

# Commands Used

```bash
ls -l

mkdir permission-lab

cd permission-lab

touch secret.txt

echo "Infrastructure Security Path" > secret.txt

cat secret.txt

chmod 000 secret.txt

cat secret.txt

whoami

id

sudo useradd analyst

sudo passwd analyst

sudo chown analyst secret.txt

su - analyst

who

w

ls -ld /root

ls -ld /home
```

---

# Evidence

## Creating the Permission Lab

![Permission Lab](screenshots/mkdir.png)

---

## Creating and Reading the File

![Create File](screenshots/touch.png)

---

## Removing Permissions with chmod

![chmod](screenshots/chmod.png)

---

## Permission Denied Investigation

![Permission Denied](screenshots/denied)

---

## Nano Permission Error

![Nano Error](screenshots/permission-denied.png)

---

## User and Group Information

![whoami and id](screenshots/whoami-id.png)

---

## Creating a New Linux User

![useradd](screenshots/useradd.png)

--- 

## Protected Directories

![Protected Directories](screenshots/ls-ld.png)

---

# Troubleshooting Performed

I intentionally removed all permissions from a file using:

```bash
chmod 000 secret.txt
```

After that, Linux denied access to the file.

I investigated:

- File permissions
- Ownership
- Current user
- Groups
- Directory permissions

Then I restored permissions and ownership to recover access.

---
