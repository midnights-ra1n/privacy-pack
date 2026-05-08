# Browser Extensions
> 🟢 Beginner - Keep it minimal. More extensions = larger fingerprint.

## The Rule
Install only what you need. Each extension makes your browser more uniquely identifiable.

## Essential

### uBlock Origin 🟢
The most impactful extension. Blocks ads, trackers, malware at the network level.
- Firefox: full support ✅
- Chromium: reduced capability (MV3) ⚠️ instead I recommend use Brave or Vivaldi if you want keep a Chromium base
- [github.com/gorhill/uBlock](https://github.com/gorhill/uBlock)

## Useful Additions
- **LocalCDN** serves CDN resources locally, prevents CDN tracking
- **Cookie AutoDelete** deletes cookies when you close a tab
- **Firefox Multi-Account Containers** (Firefox only) isolates browsing contexts
- **ClearURLs** Remove trackers from URLs.
    > When using ClearURLs and you want login with Claude AI by sent mail link, you must disable extension or you can't loggin to your account. For now, there is not white list option.
- **Canvas Blocker - Fingerprint Protect** Prevent HTML canvas element from generating a unique identification key to protect user's privacy

## Avoid
- HTTPS Everywhere is deprecated, browsers handle this natively
- Privacy Badger creates unique fingerprint; uBlock covers the use case
- VPN browser extensions are proxies, not real VPNs