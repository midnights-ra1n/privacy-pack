# File Encryption
> 🟡 Intermediate

## Tools

### VeraCrypt 🟡
Encrypted containers or full partition encryption. Supports hidden volumes (plausible deniability).
- Cross-platform: Windows, macOS, Linux
- [veracrypt.fr](https://veracrypt.fr)

### Cryptomator 🟢
Encrypts files before cloud sync. Works with any provider (Dropbox, Google Drive, etc.).
- Per-file encryption, efficient syncing
- [cryptomator.org](https://cryptomator.org)

### LUKS (Linux)
Full disk encryption built into Linux. Set up at install time.

## Which to Use?
| Scenario | Tool |
|----------|------|
| New Linux install | LUKS at install |
| Cloud files | Cryptomator |
| Portable encrypted container | VeraCrypt |
| Specific sensitive files | VeraCrypt or GPG |
