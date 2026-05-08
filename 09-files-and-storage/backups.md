# Backups
> 🟢 Beginner concept / 🟡 Intermediate implementation

## The 3-2-1 Rule
- **3** copies of your data
- **2** different storage media
- **1** copy offsite

## Tools

### Restic 🟡
Encrypted backup to local storage, SFTP, S3, Backblaze B2, and more.
```bash
restic -r /path/to/repo init
restic -r /path/to/repo backup ~/Documents
```

### BorgBackup 🟡
Deduplicating, compressed, encrypted backups.

### Simple Options 🟢
- macOS: Time Machine + Backblaze Personal Backup
- Any platform: Syncthing for sync between devices (not a backup, a complement)

## Key Points
- Always encrypt your backups
- Test your restores regularly
- Automate - manual backups are backups that don't happen
