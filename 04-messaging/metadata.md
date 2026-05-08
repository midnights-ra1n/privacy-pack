# Metadata
> 🟢 Beginner

## What Is Metadata?
Not the content, but the context: who you talked to, when, how often, from where.

Metadata can be more revealing than content. Calling a doctor at 2am reveals a health concern even without the conversation.

## What Leaks Metadata
- Standard email (sender, recipient, subject always visible)
- SMS/calls (carrier logs everything)
- Most chat apps (server sees message graph)
- Photos (EXIF contains GPS, device, timestamp)

## Tools That Minimize Metadata
- **Signal** minimal metadata, sealed sender
- **SimpleX** designed around metadata minimization, no user IDs
- **Tor** hides network-level metadata

## Remove Metadata from Photos
- `exiftool -all= photo.jpg` (Linux/macOS)
- Scrambled Exif (Android)
- Metapho (iOS)