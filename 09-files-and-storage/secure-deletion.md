# Secure Deletion
> 🟢 Beginner concept / 🟡 Intermediate for SSDs

## Why the Trash Doesn't Delete Anything
Deleting only removes the file reference. The data stays until overwritten. Recovery tools can restore it easily.

## HDDs
Overwriting is effective:
- `shred -vuz sensitive-file.txt` (Linux/macOS)
- BleachBit (cross-platform GUI)

## SSDs: It's Different
Wear-leveling means `shred` is unreliable on SSDs.

Better approaches:
- Use **full disk encryption from the start** format wipes the key, data is unrecoverable
- Manufacturer's ATA Secure Erase tool
- Physical destruction for sensitive drives

## Before Selling a Device
- With FDE enabled: format and reinstall encrypted data is unrecoverable
- Without FDE: ATA Secure Erase or physical destruction
- macOS: Disk Utility → Erase with Security Options slider
