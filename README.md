# ![alt text](./media/linux-logo.png?raw=true) Linux Commands Reference

## Introduction

Welcome to the Linux Commands Reference! 

This reference lists the commonly used commands and is not exhaustive. Where available, the individual command files will provide examples of usage for your reference. Linux commands have various options and arguments. It's essential to consult the Linux command's [manual page](https://www.linux.org/forums/linux-beginner-tutorials.123) for detailed information and usage. Enjoy!

## Commands

### Disk Management
- `fdisk` - Partition table manipulator.
- `mkfs` - Create a file system.
- `mount` - Mount a file system.
- `umount` - Unmount a file system.
- `df` - Display disk space usage.
- `du` - Estimate file and directory space usage.
- `fsck` - File system consistency check.
- `badblocks` - Check for bad blocks on a disk.

### Text Processing
- `cat` - Concatenate and display file content.
- `grep` - Search text using patterns.
- `sed` - Stream editor for text manipulation.
- `awk` - Text processing tool.
- `sort` - Sort lines in text files.
- `uniq` - Remove duplicate lines.
- `cut` - Remove sections from lines.
- `tr` - Translate or delete characters.
- `wc` - Word, line, character, and byte count.

### System Monitoring
- `top` or `htop` - Display system and process information.
- `vmstat` - Virtual memory statistics.
- `iostat` - Input/output statistics.
- `sar` - Collect and report system activity.
- `ps` - List running processes.
- `watch` - Execute a program periodically.

### File Transfer
- `scp` - Securely copy files between hosts.
- `rsync` - Synchronize files and directories.
- `ftp` - File Transfer Protocol client.
- `sftp` - Secure FTP client.
- `ncftp` - Improved FTP client.
- `curl` - Transfer data with URLs.
- `wget` - Download files from the internet.

### File and Directory Operations
- `ls` - List files and directories.
- `cd` - Change directory.
- `pwd` - Print current working directory.
- `mkdir` - Create a new directory.
- `rm` - Remove files and directories.
- `cp` - Copy files and directories.
- `mv` - Move/rename files and directories.
- `touch` - Create an empty file or update file timestamps.
- `cat` - View the contents of a file.
- `head` - Display the first few lines of a file.
- `tail` - Display the last few lines of a file.
- `ln` - Create links between files.
- `find` - Search for files and directories.

### File Permissions and Ownership
- `chmod` - Change file permissions.
- `chown` - Change file ownership.
- `chgrp` - Change group ownership.
- `umask` - Set default permissions.
- `sudo` - Execute a command as another user.
- `su` - Switch to another user.
- `visudo` - Edit sudoers file.

### System Configuration
- `hostname` - Display or set the system's hostname.
- `date` - Display or set the system date and time.
- `timedatectl` - Control the system's time and date.
- `locale` - Display or set the system locale.
- `passwd` - Change user password.
- `shutdown` - Shutdown or restart the system.
- `reboot` - Reboot the system.

### Network Configuration
- `ifconfig` or `ip` - Configure network interfaces.
- `route` - Display or modify the routing table.
- `netstat` - Display network statistics.
- `iptables` - Configure firewall rules (legacy).
- `ufw` - Uncomplicated Firewall (UFW) management.
- `firewalld` - Firewall management (systemd-based).

### Text Editors
- `nano` - Simple text editor.
- `vim` or `vi` - Powerful text editor.
- `emacs` - Extensible text editor.
- `gedit` - GNOME text editor.
- `kate` - KDE text editor.
- `sublime-text` - Sublime Text editor.

### Disk Usage Analysis
- `du` - Estimate file and directory space usage.
- `ncdu` - NCurses Disk Usage - interactive disk usage analyzer.
- `df` - Display disk space usage.
- `baobab` - GNOME Disk Usage Analyzer.

### Archive Management
- `tar` - Create and extract tar archives.
- `gzip` or `gunzip` - Compress and decompress files.
- `bzip2` or `bunzip2` - Compress and decompress files.
- `zip` or `unzip` - Create and extract zip archives.
- `rar` or `unrar` - Create and extract rar archives.
- `7z` or `7za` - Create and extract 7z archives.
- `xz` or `unxz` - Compress and decompress files with LZMA algorithm.
- `ar` or `tar` - Archive manipulation.

### User Management
- `useradd` - Add a new user.
- `userdel` - Delete a user.
- `usermod` - Modify user settings.
- `passwd` - Change user password.
- `groupadd` - Add a new group.
- `groupdel` - Delete a group.
- `groups` - Display groups a user belongs to.
- `id` - Display user and group information.

### Network Troubleshooting
- `ping` - Send ICMP echo requests.
- `traceroute` - Trace the route to a host.
- `netstat` - Display network statistics.
- `dig` - DNS lookup utility.
- `nslookup` - Query DNS records.
- `host` - DNS lookup tool.
- `ifconfig` - Configure network interfaces.

### System Backup and Restore
- `tar` - Create and extract backups.
- `rsync` - Synchronize files and directories.
- `dd` - Copy and convert files.
- `dump` and `restore` - Backup and restore filesystems.

### Package Management
- `apt-get` - Debian/Ubuntu package manager.
- `apt` - Advanced package tool (Debian/Ubuntu).
- `yum` or `dnf` - CentOS/Fedora package manager.
- `rpm` - RPM package manager (Red Hat).
- `dpkg` - Debian package manager.
- `zypper` - OpenSUSE package manager.
- `snap` - Snap package manager (Ubuntu).

### System Logging
- `journalctl` - Query the systemd journal.
- `syslog` - System log daemon.
- `logrotate` - Log rotation utility.
- `dmesg` - Display kernel messages.
- `tail` - Display the end of log files.

### System Information
- `uname` - Display system information.
- `lsb_release` - Display Linux Standard Base information.
- `lscpu` - Display CPU information.
- `lsblk` - List block devices.
- `lshw` - List hardware information.
- `inxi` - Display system information.

### Shell Scripting
- `echo` - Display text.
- `if` - Conditional statements.
- `for` - Looping constructs.
- `while` - Looping constructs.
- `case` - Evaluate conditional cases.
- `grep` - Search text using patterns.
- `sed` - Stream editor for text manipulation.
- `awk` - Text processing tool.
- `cut` - Remove sections from lines.
- `tee` - Redirect output to files and pipes.
- `xargs` - Build and execute command lines from input.

### Disk Management
- `fdisk` - Partition table manipulator.
- `gdisk` or `parted` - GUID Partition Table (GPT) tools.
- `mkfs` - Create a file system.
- `fsck` - File system consistency check.
- `mount` - Mount a file system.
- `umount` - Unmount a file system.
- `blkid` - Display block device attributes.
- `swapon` and `swapoff` - Enable and disable swap space.

### File Searching
- `find` - Search for files and directories.
- `locate` - Quickly find files by name.
- `which` - Display the path to an executable.
- `whereis` - Locate binary, source, and manual page files.
- `grep` - Search text using patterns.

## License
The content of this project itself is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International license](https://creativecommons.org/licenses/by-sa/4.0/), and the underlying source code used to format and display that content is licensed under the [MIT license](LICENSE).
