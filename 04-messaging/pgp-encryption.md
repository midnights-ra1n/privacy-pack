# PGP Encryption
> 🟡 Intermediate

## How It Works
PGP uses a key pair: a **public key** for others to encrypt messages to you, and a **private key** to decrypt them.

## Basic GPG Commands
```bash
gpg --full-generate-key
gpg --export --armor you@email.com > public.asc
gpg --encrypt --recipient them@email.com file.txt
gpg --decrypt file.txt.gpg
```

## Best Practices
- Strong passphrase on your private key
- Set an expiration date (1–2 years)
- Create a revocation certificate immediately
- Back up your private key securely, offline

## Limitations
- Encrypts content but not metadata
- Complex UX - most users are better served by Signal or Proton Mail
