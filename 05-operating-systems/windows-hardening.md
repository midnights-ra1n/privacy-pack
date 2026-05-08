# Windows Hardening
> 🟡 Intermediate - For those who can't switch to Linux.

> I recommend you to install or switch Windows 11 LTSC 2024 because there are no Microsoft Store apps. Also use [Chris Titus Windows Utility](https://christitus.com/windows-tool/) to disable the lot of useless options of Windows.

## Core Issues
- Significant telemetry by default
- Microsoft account required (can be bypassed)
- Advertising ID, Cortana, diagnostics all enabled

## Quick Wins
- **O&O ShutUp10++** — free GUI tool to disable telemetry and data collection
  [oo-software.com/shutup10](https://www.oo-software.com/en/shutup10)
- **Use a local account** — disconnect from internet during setup to skip Microsoft account

## Key Settings
- Settings → Privacy & Security → Diagnostics → set to "Required only"
- Settings → Privacy & Security → General → disable advertising ID
- Disable Cortana

## Encryption
Enable **BitLocker** (Pro) or **Device Encryption** (Home). Store recovery key offline, not only in Microsoft account.

## Additional Tools
- **Portmaster** - application-level firewall
- **Windows Sandbox** (Pro built-in) - disposable VM for testing software
