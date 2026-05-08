# Encrypted DNS
> 🟡 Intermediate

## Protocols
- **DoH** - inside HTTPS, port 443, hard to block, best for browsers
- **DoT** - dedicated TLS, port 853, better for router/system config
- **DoQ** - QUIC-based, faster, limited support

## Configuration

### Firefox
Settings → Privacy & Security → DNS over HTTPS → Custom URL

### Chrome/Brave
Settings → Security → Use secure DNS

### System-wide (Linux, systemd-resolved)
```ini
# /etc/systemd/resolved.conf
[Resolve]
DNS=9.9.9.9
DNSOverTLS=yes
```

### Router
Configure in router DNS settings. OPNsense and pfSense support this natively.

## Limitations
Encrypted DNS hides query content, but SNI in TLS still reveals domains to your ISP. A VPN is needed to hide traffic at the network level.
