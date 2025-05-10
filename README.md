# 🐧 Linux Learning Notes (Simple & Sequential)

---

### 1. Introduction to Linux
**What is Linux? History and Evolution**  
Linux is a free and open-source operating system created by Linus Torvalds in 1991. It is based on Unix and is known for stability, security, and flexibility. Over time, it has become the backbone of servers, cloud platforms, and embedded systems.

**Linux vs Unix**  
- Unix is a proprietary OS from the 1970s.  
- Linux is open-source, Unix-like, and widely used in modern computing.  
- Linux is flexible, community-driven, and cloud-ready.

**Open Source Licensing (GPL)**  
Linux is licensed under the GNU GPL, which means users can freely use, modify, and share it.

**Where Linux is Used**  
- Servers, Cloud, Mobile, Desktops, Supercomputers, IoT

---

### 2. Linux Architecture
**Kernel Space vs User Space**  
- Kernel: Core part with full access to hardware.  
- User: Applications run here, separated from kernel.

**System Calls**  
Interface for user programs to request services from the kernel (`read()`, `write()`).

**Init Systems**  
- SysVinit: Older script-based boot.  
- systemd: Modern boot manager with faster startup.

**Process Creation**  
- `fork()`: Duplicates a process.  
- `exec()`: Replaces current process with new one.

---

### 3. File System & Directories
**Directory Structure (FHS)**  
- `/etc`: Configs  
- `/var`: Logs, temp files  
- `/home`: User folders  
- `/proc`, `/sys`: Virtual system info  
- `/dev`: Device nodes

**Mounting and fstab**  
- `mount`: Attach drives  
- `/etc/fstab`: Automount settings

---

### 4. Basic Linux Commands
**File Commands**: `cp`, `mv`, `rm`, `mkdir`, `touch`  
**File Viewing**: `cat`, `less`, `head`, `tail`  
**Text Tools**: `grep`, `awk`, `sed`, `cut`  
**Monitoring**: `top`, `htop`, `ps`, `vmstat`, `iostat`  
**Find Files**: `find`, `locate`, `xargs`, `which`

---

### 5. Users and Permissions
**Create Users/Groups**: `useradd`, `groupadd`, `passwd`, `id`  
**Permissions**: `chmod`, `chown`, `umask`  
**Special Bits**: SUID, SGID, Sticky Bit  
**ACLs**: `getfacl`, `setfacl`

---

### 6. Process Management
**Jobs**: `&`, `jobs`, `fg`, `bg`, `ctrl+z`  
**Signals**: `kill`, `nice`, `renice`  
**Process Tree**: `pstree`, `htop`

---

### 7. Package Management
**Debian**: `apt`, `dpkg`  
**RHEL**: `yum`, `dnf`, `rpm`  
**Others**: `snap`, `flatpak`, source install

---

### 8. Networking
**Interfaces**: `ip`, `ifconfig`, `nmcli`  
**DNS/Routing**: `resolv.conf`, `route`  
**Tools**: `ping`, `netstat`, `ss`, `nmap`, `tcpdump`, `iptables`

---

### 9. Shell Scripting & Automation
**Basics**: Variables, Conditionals, Loops  
**Cron Jobs**: `crontab -e`  
**Functions & Exit Codes**: `function name {}`, `$?`

---

### 10. systemd & Services
**Service Commands**: `systemctl start/stop/status`  
**Units & Targets**: service, timer, `multi-user.target`  
**Journaling**: `journalctl`, log rotation

---

### 11. Disks, Partitions & LVM
**Tools**: `lsblk`, `fdisk`, `parted`, `mkfs`, `mount`, `df`, `du`  
**LVM**: PV, VG, LV creation  
**RAID**: `mdadm` for software RAID

---

### 12. Linux Security
**File Permissions**: Basic & special bits  
**Firewalls**: `iptables`, `firewalld`  
**Access Control**: SELinux, AppArmor  
**sudo/su/PAM**: Access & authentication

---

### 13. Logs & Troubleshooting
**System Logs**: `/var/log/messages`, `auth.log`  
**Kernel Logs**: `dmesg`, `auditd`  
**Logrotate**: Auto log rotation  
**Troubleshooting**: Log analysis and issue tracing

---

### 14. Performance Tuning
**Monitoring Tools**: `top`, `htop`, `vmstat`, `iostat`, `iotop`  
**Kernel Tuning**: `sysctl`  
**Swap & Hugepages**: `swapon`, `free`, `/etc/sysctl.conf`

---

### 15. Linux in Cloud & Containers
**Linux in Cloud**: AWS, GCP, Azure, cloud-init  
**Containers**: Docker, Podman basics  
**Kubernetes**: Linux nodes, kubelet, cgroups

---

✔️ Keep learning by doing. Use VMs, online labs like Katacoda, or set up your own Linux lab!
