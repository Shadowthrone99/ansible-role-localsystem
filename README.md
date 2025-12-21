# ansible-role-localsystem
Local Ubuntu 24.04 workstation bootstrap role
[README.md](https://github.com/user-attachments/files/24279389/README.md)
# localsystem

An Ansible role to bootstrap and configure a **local Ubuntu 24.04 LTS workstation**
with common desktop, development, cloud, security, and virtualization tooling.

##  Features

- Core networking and system utilities
- GNOME desktop tools and tweaks
- Google Chrome
- Google Cloud CLI + GKE auth plugin
- kubectl
- Insync
- VirtualBox 7.1
- TeamViewer
- ClamAV with automatic signature updates
- Clean, modular, tagged execution

## Supported Platforms

- Ubuntu 24.04 LTS (Noble)
- ansible-core ≥ 2.19

## Role Variables

```yaml
clamav_update_on_install: true
apt_autoremove: true
apt_autoclean: true




Installed Packages (high-level)

Google Chrome
Google Cloud SDK
kubectl
VirtualBox
TeamViewer
GNOME utilities
ClamAV / ClamTK


Usage

Playbook example

- hosts: localhost
  become: true
  roles:
    - localsystem


Run with tags

ansible-playbook site.yml --tags google
ansible-playbook site.yml --tags security
ansible-playbook site.yml --tags virtualization


Idempotency

This role is fully idempotent and safe to re-run.



License
MIT


---

# .gitignore

```gitignore
*.retry
*.log
.vscode/
.idea/
.DS_Store


