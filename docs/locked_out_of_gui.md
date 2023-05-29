# Locked out of Proxmox Gui

## Resources
- https://forum.proxmox.com/threads/proxmox-ve-login-failed-please-try-again.55488/page-2

## GUI 👎, SSH 👍
```bash

systemctl stop pve-cluster corosync
pmxcfs -l
rm /etc/corosync/*
rm /etc/pve/corosync.conf
killall pmxcfs
systemctl start pve-cluster
```
