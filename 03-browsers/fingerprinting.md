# Browser Fingerprinting
> 🟡 Intermediate

## What Is It?
Websites identify you by collecting browser attributes (screen resolution, fonts, timezone, GPU, plugins) that form a unique profile - no cookies needed.

## Common Techniques
- Canvas/WebGL fingerprinting GPU rendering differences create unique hashes
- WebRTC can leak your real IP even behind a VPN
- Font enumeration
- User-Agent and header analysis

## Test Yourself
- [coveryourtracks.eff.org](https://coveryourtracks.eff.org)
- [browserleaks.com](https://browserleaks.com)

## How to Reduce It
- Use Mullvad Browser or Tor Browser (designed for uniformity)
- Enable `privacy.resistFingerprinting` in Firefox
- Disable WebRTC
- Don't resize the browser window
- Avoid stacking many extensions

## The Paradox
Trying hard to be unique-free with many tools can itself make you more unique. Uniformity (looking like everyone else) beats suppression.
