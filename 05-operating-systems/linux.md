# Linux for Privacy
> 🟡 Intermediate

## Why Linux?
- Open-source and auditable
- No mandatory telemetry or cloud account
- Full control over running processes and network
- Easy full disk encryption setup at install

## Distro Recommendations
| Distro | Level | Use Case |
|--------|-------|----------|
| [Fedora](https://fedoraproject.org) | 🟢 | Daily use, modern hardware |
| [Debian](https://debian.org) | 🟡 | Stable, server, long-term |
| [Tails](https://tails.boum.org) | 🔴 | Amnesic, USB-only, routes via Tor |
| [Whonix](https://whonix.org) | 🔴 | Tor-based VM setup |
| [Qubes OS](https://qubes-os.org) | ⚫ | Compartmentalization via VMs |

## Key Practices
- Enable **LUKS full disk encryption** at install
- Keep system updated
- Use UFW firewall: `sudo ufw enable && sudo ufw default deny incoming`
- Use Flatpak for sandboxed app permissions
