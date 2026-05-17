# Linux System Exploration Lab

## Objective

Explore the Linux filesystem, users, processes, logs, and system monitoring tools to understand how Linux is organized 
and how infrastructure troubleshooting begins.

## Technologies Used

- AlmaLinux
- VirtualBox
- Apache

## Topics Covered

- Linux filesystem navigation
- Hidden files
- System directories
- Logs
- Running processes
- System monitoring
- Linux users

This lab helped me understand Linux as an organized system where directories, users, processes, and logs interact.
This is an important foundation for infrastructure security, troubleshooting, and monitoring.


## Commands Used

```bash
pwd
ls -al
tree /home
journalctl -u httpd
tail -f /var/log/httpd/access_log
ps aux
ps aux | grep httpd
top
whoami
id
cat /etc/passwd
```

