# Bash-to-root 🚀

## Introduction to Linux
Linux is an open-source, Unix-like operating system that powers a wide range of devices, from personal computers to servers and embedded systems. It is known for its stability, security, and flexibility.
### Features of Linux:
- Open-source and free
- Multi-user and multitasking
- Secure and stable
- Customizable (various distributions available)
- Strong community support
## Installing Linux
There are multiple ways to install Linux, depending on the distribution and the system requirements.

### 1. Choosing a Linux Distribution
Popular Linux distributions include:
- **Ubuntu** - Beginner-friendly and widely used
- **Fedora** - Cutting-edge features with stability
- **Debian** - Reliable and community-driven
- **Arch Linux** - Highly customizable, for advanced users
- **CentOS/Rocky Linux** - Enterprise-grade stability

### 2. Installation Methods
#### a) Installing Linux on a PC
1. **Download the ISO** file of your chosen Linux distribution from the official website.
2. **Create a bootable USB drive** using tools like Rufus (Windows) or `dd` (Linux/Mac).
3. **Boot from the USB drive** by selecting it in the BIOS/UEFI boot menu.
4. **Follow the installation prompts**, including partitioning, user creation, and software selection.
5. **Restart and log in** to your new Linux system.

#### b) Installing Linux in a Virtual Machine
1. Install a virtualization tool like VirtualBox or VMware.
2. Create a new virtual machine and allocate resources.
3. Mount the Linux ISO as a boot disk.
4. Follow the installation steps as for a physical machine.

#### c) Dual Booting with Windows
1. Shrink an existing Windows partition to free space.
2. Follow the standard installation steps and select "Install alongside Windows."
3. Configure the bootloader (GRUB) to manage both operating systems.
## Basic Linux Commands
Below are some fundamental Linux commands that every user should know:
### 1. File and Directory Commands:
- `ls` - List files and directories
- `pwd` - Print the current working directory
- `cd <directory>` - Change directory
- `mkdir <directory>` - Create a new directory
- `rmdir <directory>` - Remove an empty directory
- `rm <file>` - Remove a file
- `rm -r <directory>` - Remove a directory and its contents
- `cp <source> <destination>` - Copy files or directories
- `mv <source> <destination>` - Move or rename files and directories
### 2. File Permission Commands:
- `chmod <permissions> <file>` - Change file permissions
- `chown <user>:<group> <file>` - Change file ownership
### 3. Process Management:
- `ps` - Display active processes
- `top` - Show real-time process activity
- `kill <PID>` - Terminate a process by its ID
- `killall <process_name>` - Kill all processes by name
### 4. System Monitoring:
- `df -h` - Show disk space usage
- `du -sh <directory>` - Show size of a directory
- `free -m` - Display memory usage
- `uptime` - Show system uptime
- `who` - Show who is logged in
### 5. Networking Commands:
- `ifconfig` or `ip a` - Display network interfaces
- `ping <host>` - Check connectivity to a host
- `netstat -tulnp` - Show active network connections
- `wget <URL>` - Download files from the web
## Difference Between Unix and Linux
| Feature          | Unix                                       | Linux                                      |
|-----------------|---------------------------------|--------------------------------|
| Origin         | Developed in the 1970s at AT&T Bell Labs | Inspired by Unix, developed by Linus Torvalds in 1991 |
| Open-source    | Mostly proprietary, some open-source variants exist | Fully open-source and freely available |
| Distributions  | Various commercial versions (AIX, HP-UX, Solaris) | Multiple distributions (Ubuntu, Fedora, CentOS, Arch) |
| Customizability | Limited due to licensing restrictions | Highly customizable and flexible |
| Usage          | Mainly used in enterprises and mainframes | Used in personal computers, servers, IoT devices |

# 50 Basic Linux Commands

## 📂 File and Directory Management
1. `ls` – List files and directories  
2. `cd` – Change directory  
3. `pwd` – Print working directory  
4. `mkdir` – Create a new directory  
5. `rmdir` – Remove an empty directory  
6. `rm -r` – Remove a directory and its contents  
7. `cp` – Copy files and directories  
8. `mv` – Move or rename files  
9. `touch` – Create an empty file  
10. `find` – Search for files in a directory  
11. `locate` – Find the location of a file  
12. `stat` – Display detailed information about a file  
13. `tree` – Show directory structure  

## 📄 File Operations
14. `cat` – View the contents of a file  
15. `tac` – View a file in reverse order  
16. `less` – View large files page by page  
17. `head` – Show the first 10 lines of a file  
18. `tail` – Show the last 10 lines of a file  
19. `grep` – Search for patterns in a file  
20. `awk` – Pattern scanning and text processing  
21. `sed` – Stream editor for modifying text  
22. `diff` – Compare two files line by line  
23. `sort` – Sort the contents of a file  
24. `uniq` – Remove duplicate lines from a file  
25. `wc` – Count lines, words, and characters in a file  

## 🖥️ System Information
26. `uname -a` – Show system information  
27. `hostname` – Display or set the hostname  
28. `uptime` – Show how long the system has been running  
29. `whoami` – Display the current user  
30. `id` – Show user and group IDs  
31. `df -h` – Check disk space usage  
32. `du -sh` – Show disk usage of a directory  
33. `free -h` – Show memory usage  
34. `top` – Display running processes  
35. `htop` – Interactive process viewer (needs installation)  

## 🔧 Process and User Management
36. `ps aux` – Show all running processes  
37. `kill <PID>` – Terminate a process by its ID  
38. `killall <name>` – Kill all processes by name  
39. `pkill <name>` – Kill processes by name  
40. `nice` – Start a process with a given priority  
41. `renice` – Change the priority of a running process  
42. `useradd <username>` – Add a new user  
43. `passwd <username>` – Change user password  
44. `who` – Show logged-in users  
45. `w` – Show active users and what they are doing  

## 🔒 Permissions and Ownership
46. `chmod` – Change file permissions  
47. `chown` – Change file ownership  
48. `chgrp` – Change file group ownership  

## 🚀 Networking

## 1. Network Configuration and Status

- **Check IP address:**
  ```sh
  ip a
  ```
  ```sh
  ifconfig  # Deprecated but still available
  ```

- **Check routing table:**
  ```sh
  ip r
  ```
  ```sh
  route -n  # Older command
  ```

- **Check active network connections:**
  ```sh
  netstat -tulnp
  ```
  ```sh
  ss -tulnp  # Preferred over netstat
  ```

## 2. Network Diagnostics

- **Ping a host:**
  ```sh
  ping example.com
  ```

- **Traceroute to a destination:**
  ```sh
  traceroute example.com
  ```
  ```sh
  tracepath example.com  # Alternative command
  ```

- **Check DNS resolution:**
  ```sh
  nslookup example.com
  ```
  ```sh
  dig example.com
  ```

- **Test network connectivity:**
  ```sh
  curl -I http://example.com
  ```
  ```sh
  wget --spider http://example.com
  ```

## 3. Network Interfaces Management

- **Bring an interface up or down:**
  ```sh
  ip link set eth0 up
  ip link set eth0 down
  ```
  ```sh
  ifconfig eth0 up  # Deprecated
  ifconfig eth0 down
  ```

- **Restart networking service:**
  ```sh
  systemctl restart networking
  ```
  ```sh
  service networking restart
  ```

## 4. Port and Firewall Management

- **Check open ports:**
  ```sh
  netstat -tulnp
  ```
  ```sh
  ss -tulnp
  ```

- **Manage firewall rules with UFW:**
  ```sh
  ufw status
  ufw allow 22/tcp
  ufw deny 80/tcp
  ufw enable
  ufw disable
  ```

- **Manage firewall rules with iptables:**
  ```sh
  iptables -L
  iptables -A INPUT -p tcp --dport 22 -j ACCEPT
  iptables -A INPUT -p tcp --dport 80 -j DROP
  ```

## 5. Network Monitoring

- **Monitor network traffic:**
  ```sh
  tcpdump -i eth0
  ```

- **Display network statistics:**
  ```sh
  ifstat
  ```
  ```sh
  vnstat
  ```

## 6. File Transfer and Remote Access

- **Securely copy files:**
  ```sh
  scp file.txt user@remote:/path/
  ```

- **Synchronize directories:**
  ```sh
  rsync -avz /local/dir user@remote:/remote/dir
  ```

- **Connect to a remote machine via SSH:**
  ```sh
  ssh user@remote
  ```

These are fundamental commands for working with Linux. Mastering them will improve your efficiency in the Linux environment! 🚀
