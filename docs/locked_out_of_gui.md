# Locked out of Proxmox Gui

## GUI 👎, SSH 👍
```bash

systemctl stop pve-cluster
rm -f /var/lib/pve-cluster/.pmxcfs.lockfile
systemctl start pve-cluster
```
