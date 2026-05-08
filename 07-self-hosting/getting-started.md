# Self-Hosting: Getting Started
> 🟡 Intermediate

## Why Self-Host?
- Your data stays on your hardware
- No subscription fees
- No vendor lock-in or account termination risk

## What You Need
- **Hardware:** Raspberry Pi, old PC, mini PC, or a VPS
- **OS:** Debian or Ubuntu Server
- **Skills:** SSH, basic Linux command line, networking basics

## VPS vs Home Server
| | VPS | Home Server |
|--|-----|-------------|
| Cost | Monthly fee | One-time hardware |
| Privacy | Provider can access | You control |
| Availability | High | Depends on uptime |

## Core Stack
- **Reverse proxy:** Caddy or Nginx Proxy Manager (auto HTTPS)
- **Containers:** Docker + Docker Compose

## Commonly Self-Hosted Services
| Service | Replaces | Link |
|---------|----------|------|
| Vaultwarden | Bitwarden cloud | [github](https://github.com/dani-garcia/vaultwarden) |
| Nextcloud | Google Drive | [nextcloud.com](https://nextcloud.com) |
| Immich | Google Photos | [immich.app](https://immich.app) |
| AdGuard Home | NextDNS | [adguard.com](https://adguard.com/adguard-home.html) |
| Syncthing | Dropbox sync | [syncthing.net](https://syncthing.net) |
| SearXNG | Google Search | [searxng.org](https://searxng.org) |
| FreshRSS | Feedly | [freshrss.org](https://freshrss.org) |
| Matrix/Synapse | Slack/Discord | [matrix.org](https://matrix.org) |
| Navidrome | Spotify or Apple Music | [navidrome.org](https://www.navidrome.org/) |
