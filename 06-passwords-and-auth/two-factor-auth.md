# Two-Factor Authentication (2FA)
> 🟢 Beginner

## Methods (Best to Worst)
| Method | Security | Notes |
|--------|----------|-------|
| Hardware key (FIDO2) | ⚫ Excellent | YubiKey — phishing-proof |
| TOTP app | 🔴 Strong | Aegis (Android), Raivo (iOS) |
| Email OTP | 🟡 Moderate | Depends on email security |
| SMS OTP | 🟢 Weak | Vulnerable to SIM swapping |

## SMS 2FA: Why It's Weak
SIM swapping - attacker transfers your number to their SIM via social engineering your carrier lets them intercept your SMS codes.

## TOTP Apps
- **Aegis** (Android) - open-source, encrypted vault, export feature
- **Raivo** (iOS) - open-source
- **Ente Auth** - cross-platform, optional encrypted sync

## Hardware Keys
- **YubiKey** - widely supported
- **Nitrokey** - open-source hardware alternative

Back up TOTP seeds when setting up 2FA.
