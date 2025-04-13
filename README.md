# 🐧 Useful Linux Commands Cheat Sheet

A categorized and extensible collection of essential Linux commands for developers, sysadmins, and power users. Perfect for quick reference and GitHub documentation.

---

## 📁 Directory & File Navigation

| Command | Description |
|---------|-------------|
| `ls -la` | List all files and directories with permissions |
| `cd /path/to/dir` | Change directory |
| `pwd` | Show current directory path |
| `tree` | Display directory tree structure |
| `du -sh *` | Show human-readable size of each item in the current directory |
| `find . -type f` | List all files recursively |
| `find .` | List all files and directories recursively |
| `find . \| wc -l` | Count total files and directories (inodes used) |
| `find . -type f \| wc -l` | Count only files |
| `find . -type d \| wc -l` | Count only directories |

---

## 🧹 Disk & Inode Management

| Command | Description |
|---------|-------------|
| `df -h` | Show disk space usage (human-readable) |
| `du -sh` | Show size of the current folder |
| `du -sh * \| sort -h` | Show and sort all subfolders by size |
| `ncdu` | Interactive disk usage analyzer |
| `stat filename` | Show detailed info about a file |
| `find . -type f -name '*.log' -delete` | Delete all `.log` files recursively |

---

## 🔒 Permissions & Ownership

| Command | Description |
|---------|-------------|
| `chmod +x script.sh` | Make a script executable |
| `chmod 755 file` | Set permissions (rwx for owner, rx for others) |
| `chown user:group file` | Change file ownership |
| `ls -l` | List files with permission and ownership info |

---

## 💻 SSH & Remote Access

| Command | Description |
|---------|-------------|
| `ssh user@host` | Connect to a remote server |
| `scp file.txt user@host:/path` | Copy file to a remote server |
| `rsync -avz file/ user@host:/path/` | Sync files to remote (efficiently) |
| `ssh-keygen` | Generate an SSH key pair |
| `ssh-copy-id user@host` | Copy SSH key to remote server for passwordless login |

---

## ⚙️ Process & System Monitoring

| Command | Description |
|---------|-------------|
| `top` | Display real-time system processes |
| `htop` | Enhanced process viewer |
| `ps aux \| grep nginx` | Search for a process by name |
| `kill -9 PID` | Force kill a process by PID |
| `uptime` | Show how long the system has been running |
| `free -h` | Show memory usage |
| `vmstat` | Show system performance stats |

---

## 📦 Package Management

### Debian/Ubuntu-based:

| Command | Description |
|---------|-------------|
| `sudo apt update && sudo apt upgrade` | Update packages and OS |
| `sudo apt install package` | Install a package |
| `sudo apt remove package` | Remove a package |

### RHEL/CentOS-based:

| Command | Description |
|---------|-------------|
| `sudo yum update` | Update packages |
| `sudo yum install package` | Install a package |
| `sudo yum remove package` | Remove a package |

---

## 📂 File Compression

| Command | Description |
|---------|-------------|
| `tar -czf archive.tar.gz folder/` | Create compressed archive |
| `tar -xzf archive.tar.gz` | Extract archive |
| `zip -r archive.zip folder/` | Create ZIP archive |
| `unzip archive.zip` | Extract ZIP archive |

---

## 📝 Text Manipulation & Logs

| Command | Description |
|---------|-------------|
| `cat file.txt` | View file content |
| `head -n 20 file.txt` | First 20 lines of file |
| `tail -n 20 file.txt` | Last 20 lines of file |
| `tail -f /var/log/syslog` | Follow log file in real time |
| `grep 'search' file.txt` | Search for text in file |
| `sed -i 's/old/new/g' file.txt` | Replace text in file |
| `wc -l file.txt` | Count lines in a file |

---

## 🔁 Networking & Utilities

| Command | Description |
|---------|-------------|
| `ping domain.com` | Test network connectivity |
| `curl -I https://example.com` | Get HTTP response headers |
| `wget URL` | Download file from internet |
| `netstat -tulpn` | Show listening ports and services |
| `ss -tuln` | View open ports (modern netstat) |

---

## 🐚 Miscellaneous

| Command | Description |
|---------|-------------|
| `history` | Show command history |
| `alias ll='ls -la'` | Create an alias |
| `crontab -e` | Edit user's cron jobs |
| `whoami` | Show current user |
| `hostname -I` | Show IP address of server |

---

✅ Keep updating this list as you explore more Linux tools and commands!
