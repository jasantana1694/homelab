# Homelab

A self-hosted homelab built on Proxmox VE for learning and practicing real-world sysadmin skills.

## Infrastructure
- **Hypervisor:** Proxmox VE running on bare metal
- **Firewall:** OPNsense VM
- **Windows Server 2022 VM:** Active Directory Domain Services
- **Ubuntu Server 24.04 VM:** Nginx web server, Samba file server, Ansible

## Projects

### Active Directory
- Deployed AD DS and promoted server to domain controller
- Created departmental Organizational Units (IT, HR, Finance)
- Configured security groups and user accounts
- Wrote Group Policy Objects to enforce password policies and restrict Control Panel access
- Set up shared folders with group-based access control

### Web Server
- Deployed Nginx on Ubuntu Server 24.04
- Generated self-signed SSL certificate
- Configured HTTPS redirection from HTTP

### File Server
- Configured Samba for cross-platform network file sharing
- Accessible from both Windows and Linux clients

### Firewall
- Deployed OPNsense as a virtual firewall
- Configured WAN interface and DNS settings

### Automation
- Installed and configured Ansible
- Wrote playbooks to automate package updates and software deployment
- Configured passwordless SSH key authentication between servers

## Skills Demonstrated
- Virtualization (Proxmox VE)
- Windows Server Administration
- Active Directory & Group Policy
- Linux Server Administration
- Web Server Configuration & SSL/TLS
- Network File Sharing (Samba)
- Firewall Configuration (OPNsense)
- Infrastructure Automation (Ansible)
