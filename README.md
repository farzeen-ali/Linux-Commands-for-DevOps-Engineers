# Essential Linux Commands for DevOps Engineers 🔥

Welcome to this comprehensive guide on Linux commands essential for every DevOps engineer 🎯

This README covers commonly used commands, their important flags, and practical examples for better understanding 💡

---

## Table of Contents

- [User & Identity](#user--identity)  
- [File & Directory](#file--directory)  
- [File Permissions & Ownership](#file-permissions--ownership)  
- [Process Management](#process-management)  
- [Networking](#networking)  
- [Disk & Memory](#disk--memory)  
- [System Info & Management](#system-info--management)  
- [Package Management](#package-management)  
- [Archiving & Compressing](#archiving--compressing)  
- [Text Processing](#text-processing)  
- [Text Editors](#text-editors)  

---

## User & Identity

| Command | Description | Important Flags / Options | Usage Examples |
|---------|-------------|--------------------------|----------------|
| `whoami` | Prints current logged-in user | None | `whoami` |
| `id` | Shows user ID and groups | None | `id` |
| `passwd` | Change user password | None | `passwd` (interactive) |
| `groups` | Show groups current user belongs to | None | `groups` |

---

## File & Directory

| Command | Description | Important Flags / Options | Usage Examples |
|---------|-------------|--------------------------|----------------|
| `ls` | List directory contents | `-l` (detailed), `-a` (hidden files), `-h` (human readable sizes) | `ls -la` |
| `cd` | Change directory | None | `cd /path/to/dir` |
| `pwd` | Print current working directory | None | `pwd` |
| `mkdir` | Create directory | `-p` (create parent dirs if needed) | `mkdir -p new/dir` |
| `touch` | Create empty file or update timestamp | None | `touch file.txt` |
| `rm` | Remove file or directory | `-r` (recursive for directories), `-f` (force) | `rm -rf dir/` |
| `cp` | Copy files/directories | `-r` (recursive) | `cp file.txt backup.txt` |
| `mv` | Move or rename files/directories | None | `mv old.txt new.txt` |
| `find` | Search files/directories | `-name` (search by name), `-type` (file/dir) | `find . -name "*.log"` |

---

## File Permissions & Ownership

| Command | Description | Important Flags / Options | Usage Examples |
|---------|-------------|--------------------------|----------------|
| `chmod` | Change file permissions | `+x` (make executable), `-R` (recursive) | `chmod +x script.sh` |
| `chown` | Change file owner/group | `-R` (recursive) | `chown user:group file.txt` |
| `ls -l` | List detailed info including permissions | None | `ls -l` |

---

## Process Management

| Command | Description | Important Flags / Options | Usage Examples |
|---------|-------------|--------------------------|----------------|
| `ps` | Show running processes | `aux` (detailed all processes) | `ps aux` |
| `top` | Interactive process viewer | None | `top` |
| `kill` | Terminate a process by PID | `-9` (force kill) | `kill 1234` / `kill -9 1234` |
| `jobs` | List background jobs | None | `jobs` |
| `fg` | Bring background job to foreground | Job number | `fg %1` |
| `bg` | Resume stopped job in background | Job number | `bg %1` |

---

## Networking

| Command | Description | Important Flags / Options | Usage Examples |
|---------|-------------|--------------------------|----------------|
| `ping` | Check network connectivity | `-c` (count packets) | `ping -c 4 google.com` |
| `curl` | Transfer data from URL | `-I` (headers only), `-X` (HTTP method) | `curl -I https://example.com` |
| `ssh` | Remote login to another machine | `-p` (port), `-i` (identity file) | `ssh user@host` |

---

## Disk & Memory

| Command | Description | Important Flags / Options | Usage Examples |
|---------|-------------|--------------------------|----------------|
| `df` | Disk space usage | `-h` (human readable) | `df -h` |
| `du` | Directory/file size | `-h` (human readable), `-s` (summary) | `du -sh /var/log` |
| `free` | Memory usage | `-h` (human readable) | `free -h` |

---

## System Info & Management

| Command | Description | Important Flags / Options | Usage Examples |
|---------|-------------|--------------------------|----------------|
| `uname -a` | Show kernel and system info | None | `uname -a` |
| `uptime` | Show system uptime and load | None | `uptime` |
| `systemctl` | Manage systemd services | `start`, `stop`, `restart`, `enable`, `status` | `systemctl status nginx` |
| `journalctl` | View systemd logs | `-f` (follow) | `journalctl -f` |

---

## Package Management (Debian/Ubuntu)

| Command | Description | Important Flags / Options | Usage Examples |
|---------|-------------|--------------------------|----------------|
| `apt-get update` | Update package list | None | `sudo apt-get update` |
| `apt-get install` | Install packages | `-y` (auto yes) | `sudo apt-get install nginx -y` |
| `apt-get upgrade` | Upgrade installed packages | None | `sudo apt-get upgrade` |

---

## Archiving & Compressing

| Command | Description | Important Flags / Options | Usage Examples |
|---------|-------------|--------------------------|----------------|
| `tar` | Archive and compress files | `-c` (create), `-x` (extract), `-z` (gzip), `-v` (verbose), `-f` (file) | `tar -czvf archive.tar.gz dir/` |
| `zip` | Create zip archives | None | `zip archive.zip file1 file2` |
| `unzip` | Extract zip archives | None | `unzip archive.zip` |

---

## Text Processing

| Command | Description | Important Flags / Options | Usage Examples |
|---------|-------------|--------------------------|----------------|
| `cat` | View or create file content | `>` (redirect/overwrite), `>>` (append) | `cat file.txt` <br> `cat > file.txt` (write input to file, Ctrl+D to save) |
| `head` | View first lines of a file | `-n` (number of lines) | `head -n 10 file.txt` |
| `tail` | View last lines of a file | `-n` (number of lines), `-f` (follow new lines) | `tail -f /var/log/syslog` |
| `echo` | Print text or variables | None | `echo "Hello World"` |
| `grep` | Search text in files | `-i` (ignore case), `-r` (recursive), `-v` (invert match) | `grep -i "error" /var/log/syslog` |

---

## Text Editors

| Command | Description | Important Flags / Options | Usage Examples |
|---------|-------------|--------------------------|----------------|
| `nano` | Simple command-line text editor | None | `nano file.txt` |
| `vim` | Powerful text editor (modal) | None | `vim file.txt` |

---

## Notes on some commands

- `cat > file.txt` — allows you to create or overwrite a file by typing input directly in terminal. Press **Ctrl + D** to save and exit.  
- `touch file.txt` — creates an empty file or updates the timestamp of an existing file.  
- `chmod +x file.sh` — makes a script executable so it can be run.  
- `systemctl enable <service>` — enables a service to start on boot.

---

Feel free to ⭐ the repo if you find this helpful!  
Happy DevOps-ing! 🚀

---
