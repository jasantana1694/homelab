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
- Designed enterprise OU structure (Users, Computers, Groups, Service Accounts)
- Created departmental OUs for IT, HR, and Finance with sub-OUs for computers
- Configured security groups following AGDLP best practice
- Implemented group nesting for scalable permission management
- Delegated control to helpdesk staff following principle of least privilege
- Configured Group Policy Objects including:
  - Domain wide password and account lockout policies
  - Automatic network drive mapping for IT users
  - Control Panel restrictions for HR users
  - Desktop wallpaper enforcement for Finance users
  - Legal warning banner for IT computers
- Configured DNS with A records and CNAME records for internal name resolution
- Deployed DHCP with custom scopes and reservations
- Practiced real world scenarios including employee onboarding, offboarding, password resets, account unlocks, and new computer setup
- Used PowerShell to automate bulk user creation

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
