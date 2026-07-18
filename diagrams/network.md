# Homelab Network Diagram

## Infrastructure Overview
Internet
|
Router
|
Proxmox VE (Bare Metal)
|
|-- OPNsense VM (Firewall)
|
|-- Windows Server 2022 VM
|       - Active Directory
|       - DNS Server
|       - IT-Share (SMB)
|
|-- Ubuntu Server 24.04 VM
- Nginx (HTTPS)
- Samba File Server
- Ansible Control Node
- ## VM Specifications

| VM | OS | RAM | Storage | Role |
|---|---|---|---|---|
| opnsense-firewall | OPNsense 26.7 | 2GB | 16GB | Firewall |
| windows-server-2022 | Windows Server 2022 | 4GB | 60GB | AD DS, DNS |
| ubuntu-server-01 | Ubuntu Server 24.04 | 2GB | 32GB | Web, File, Ansible |
