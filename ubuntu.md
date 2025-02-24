# 📌 Ubuntu Commands Cheat Sheet

## 🔹 General Commands

| Command | Description | Example |
|---------|-------------|---------|
| `sudo su` | Switch to the root user with a login shell | `sudo su` |
| `ls` | List files and directories in the current directory | `ls` |
| `ls -ll` | List files with detailed info like permission, storage | `ls -ll` |
| `clear` / `cls` | Clears the current terminal screen | `clear` |
| `whoami` | Displays the current username | `whoami` |
| `hostname` | Displays the system's hostname | `hostname` |
| `hostname -i` | Shows the IP address of the system | `hostname -i` |
| `pwd` | Prints the current working directory path | `pwd` |
| `touch <file>` | Creates an empty file or updates the timestamp of a file | `touch example.txt` |
| `mkdir <dir>` | Creates a new directory | `mkdir my_folder` |
| `rm -rf <file/dir>` | Deletes files and directories recursively | `rm -rf old_folder` |
| `cat <file>` | Displays the contents of a file | `cat example.txt` |
| `cd <dir>` | Changes the current directory | `cd Documents` |
| `cd ..` | Moves up one folder | `cd ..` |
| `cp -rp <source> <destination>` | Copies files and directories | `cp -rp /home/user/file.txt /home/user/backup/` |
| `scp <file> <destination>` | Securely copies files between systems | `scp file.txt user@remote:/home/user/` |
| `mv <source> <destination>` | Moves or renames files and directories | `mv oldname.txt newname.txt` |
| `uptime` | Shows how long the system has been running | `uptime` |
| `date` | Displays current date and time | `date` |
| `cal` | Displays a calendar | `cal` |
| `history` | Displays previously executed commands | `history` |
| `whereis <command>` | Locates the binary, source, and manual files for a given command | `whereis ls` |
| `which <command>` | Shows the path to the executable file | `which python3` |

---

## 📦 Package Management

| Command | Description | Example |
|---------|-------------|---------|
| `sudo apt update` | Updates package lists | `sudo apt update` |
| `sudo apt upgrade` | Upgrades installed packages | `sudo apt upgrade` |
| `sudo apt-get install <package>` | Installs a new package | `sudo apt-get install vim` |

---

## 📁 File Compression & Extraction

| Command | Description | Example |
|---------|-------------|---------|
| `zip -r <file.zip> <folder>` | Compress files and folders recursively | `zip -r backup.zip /home/user/documents` |
| `unzip <file.zip>` | Extracts the contents of a zip file | `unzip backup.zip` |
| `tar -cvf <file.tar.gz> <folder>` | Creates a tar.gz archive | `tar -cvf archive.tar.gz /home/user/documents` |
| `tar -xvf <file.tar.gz>` | Extracts files from a tar.gz archive | `tar -xvf archive.tar.gz` |

---

## ⚙️ Process Management

| Command | Description |
|---------|-------------|
| `ps -ef` | Displays running processes |
| `grep <pattern>` | Searches for a text pattern in output |

---

## 🔍 File Search

| Command | Description |
|---------|-------------|
| `find / -name <file>` | Find a file by name from the root directory |
| `find / -type f -name <file>` | Find a specific file type |
| `find / -type d -name <dir>` | Find a directory by name |

---

## 🌐 Networking Commands

| Command | Description |
|---------|-------------|
| `ping <hostname>` | Checks network connectivity |
| `dig <hostname>` | Queries DNS information |
| `telnet <website> <port>` | Tests open ports on a remote system |
| `netstat -an` | Displays active network connections |

---

## 🔒 File Permissions & Ownership

### 📜 Permission Types

| Type | Symbol | Numeric Value | Description |
|------|--------|--------------|-------------|
| Read | `r` | 4 | Allows viewing file content |
| Write | `w` | 2 | Allows modifying the file |
| Execute | `x` | 1 | Allows running the file as a program |

### 👥 User Permission Levels

| User Type | Symbol | Description |
|-----------|--------|-------------|
| Owner | `u` | The user who owns the file |
| Group | `g` | Users who belong to the file's group |
| Others | `o` | All other users |

### 🛠️ Changing Permissions

| Command | Description | Example |
|---------|-------------|---------|
| `chmod <permissions> <file>` | Change file permissions | `chmod 755 script.sh` |
| `chmod -R 755 <dir>` | Recursively change permissions | `chmod -R 755 /var/www/html` |
| `chown <owner>:<group> <file>` | Change file ownership | `chown user:user file.txt` |
| `chown -R <owner>:<group> <dir>` | Recursively change ownership | `chown -R user:user /home/user/docs` |

### 🔢 Numeric Permission Examples

| Command | Meaning |
|---------|---------|
| `chmod 644 file.txt` | Owner: read/write, Group: read, Others: read |
| `chmod 755 script.sh` | Owner: read/write/execute, Group: read/execute, Others: read/execute |

---

## 📊 Monitoring & Performance

| Command | Description |
|---------|-------------|
| `top` | Displays real-time CPU & memory usage |
| `htop` | Interactive process viewer (alternative to top) |
| `iostat` | Displays CPU and disk usage statistics |
| `lscpu` | Shows CPU architecture details |

---

## 📥 Downloading Files

| Command | Description | Example |
|---------|-------------|---------|
| `wget <url>` | Downloads files from the internet | `wget http://example.com/file.tar.gz` |
| `curl -o <file> <url>` | Transfers data from a server | `curl -o file.tar.gz http://example.com/file.tar.gz` |

---

## 🔄 Run Levels in Linux (System Boot States)

| Run Level | Description |
|-----------|-------------|
| `init 0` | Shutdown |
| `init 1` | Single-user mode (maintenance mode) |
| `init 2` | Multi-user mode without network |
| `init 3` | Multi-user mode with network |
| `init 4` | Multi-user mode with GUI |
| `init 6` | Reboot the system |

---

🚀 **Happy Linux Commanding!**
