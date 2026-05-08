# Proxies
> 🟡 Intermediate

## Types
- **HTTP proxy** - HTTP/HTTPS only, application-level
- **SOCKS5** - protocol-agnostic, used with torrents/SSH tunneling
- **Transparent proxy** - used by ISPs, not useful for privacy

## SOCKS5 vs VPN
| | SOCKS5 | VPN |
|--|--------|-----|
| Encryption | ❌ | ✅ |
| System-wide | ❌ (per-app) | ✅ |
| Best for | Specific apps | General use |

## SSH as Proxy
`ssh -D 1080 -C -N user@your-server.com` then point your app to `localhost:1080` as SOCKS5.

## Limitations
Proxies shift your IP but don't encrypt. Use for specific limited cases, not as a privacy solution alone.
