# bash-to-root
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
## Conclusion
Linux is a powerful and flexible operating system that offers various commands for managing files, processes, and networks. Understanding these basics will help users navigate and operate Linux systems efficiently.
