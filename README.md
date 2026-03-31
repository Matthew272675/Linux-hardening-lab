# Linux-hardening-lab
This project demonstrates basic Linux system hardening techniques using an Ubuntu virtual machine. The goal was to improve system security by implementing user controls, securing remote access, enabling firewall protections, and managing file permissions.
# Linux System Hardening Lab (Ubuntu VM)
## Tools Used
- Ubuntu (VirtualBox VM)
- Linux Terminal
- UFW (Uncomplicated Firewall)
- OpenSSH Server

## Key Tasks Performed
- Created a non-root user with sudo privileges
- Secured SSH by disabling root login
- Enabled and configured UFW firewall
- Managed file permissions using chmod
- Verified system security configurations

## Commands Used
```bash
sudo adduser analyst
sudo usermod -aG sudo analyst
sudo apt install openssh-server -y
sudo nano /etc/ssh/sshd_config
sudo systemctl restart ssh
sudo ufw enable
sudo ufw allow ssh
chmod 600 secret.txt
```

## What I Learned
- Importance of least privilege access
- How to secure remote access via SSH
- Basic firewall configuration
- Linux file permission structures
- System hardening fundamentals
