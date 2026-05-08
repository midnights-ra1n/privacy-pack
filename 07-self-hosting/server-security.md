# Server Security
> 🟡 Intermediate - Essential hardening for any self-hosted server.

## SSH Hardening
Use key-based auth instead of passwords:
```bash
ssh-keygen -t ed25519 -C "your-server"
ssh-copy-id user@your-server
```

In `/etc/ssh/sshd_config`:
```
PasswordAuthentication no
PermitRootLogin no
```

## Firewall (UFW)
```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw allow ssh && sudo ufw allow 80/tcp && sudo ufw allow 443/tcp
sudo ufw enable
```

## Fail2Ban
```bash
sudo apt install fail2ban && sudo systemctl enable fail2ban --now
```
Blocks IPs after repeated failed login attempts.

## Automatic Updates
```bash
sudo apt install unattended-upgrades
sudo dpkg-reconfigure unattended-upgrades
```

## Backups (Restic)
```bash
restic -r s3:s3.amazonaws.com/my-bucket backup /path/to/data
```
Test your restores. An untested backup is an unknown backup.

## Checklist
- [ ] SSH key auth only, no root login
- [ ] UFW enabled
- [ ] Fail2ban running
- [ ] Automatic security updates enabled
- [ ] Regular encrypted offsite backups
