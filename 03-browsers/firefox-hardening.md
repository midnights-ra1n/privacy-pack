# Firefox Hardening
> 🟡 Intermediate

## Method 1: arkenfox user.js (Recommended)
Pre-configured privacy settings file. Place in your Firefox profile folder and restart.

**Repo:** [github.com/arkenfox/user.js](https://github.com/arkenfox/user.js)

Create `user-overrides.js` in the same folder for personal overrides that survive updates.

## Key about:config Tweaks
```
toolkit.telemetry.enabled = false
privacy.resistFingerprinting = true
media.peerconnection.enabled = false   # prevents WebRTC IP leak
network.dns.disablePrefetch = true
geo.enabled = false
```

⚠️ Disabling WebRTC breaks in-browser video calls.

## Multiple Profiles
`firefox --ProfileManager` - create separate profiles for work, personal, sensitive browsing.

## Easier Alternative
**LibreWolf** ships pre-configured with equivalent hardening.
