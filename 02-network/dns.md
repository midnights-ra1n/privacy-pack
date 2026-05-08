# DNS Privacy
> 🟢 Beginner - See [08-dns-filtering/](../08-dns-filtering/) for deeper coverage.

## The Problem
By default, DNS queries go to your ISP unencrypted. They can see every domain you visit even over HTTPS.

## Protocols
- **DoH** - looks like web traffic, hard to block, browser-friendly
- **DoT** - dedicated port, cleaner for router config
- **DoQ** - newer, faster, limited adoption

## Quick Setup
- **Firefox:** Settings → Privacy & Security → DNS over HTTPS
- **Chrome/Brave:** Settings → Security → Use secure DNS

## Limitations
Encrypted DNS hides query content but not the fact you're making requests. A VPN is needed to hide traffic at the network level.