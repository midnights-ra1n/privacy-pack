# DNS Blocklists
> 🟡 Intermediate

## How They Work
Blocklists contain domains known for ads, trackers, or malware. Matching queries return NXDOMAIN instead of the real IP.

## Recommended Lists

### Hagezi
Best maintained and most comprehensive option.

| List | Aggressiveness | For |
|------|---------------|-----|
| Multi Light | Low | IoT, sensitive environments |
| Multi Pro | Medium | Good daily use balance |
| Multi Pro++ | High | Recommended for most users |
| Multi Ultimate | Very High | Accept some false positives |
| [Allowlist Referral](https://adguardteam.github.io/HostlistsRegistry/assets/filter_45.txt) | N/A | Whitelisted domains |

[github.com/hagezi/dns-blocklists](https://github.com/hagezi/dns-blocklists)

### OISD
Clean, broad coverage. OISD Small (conservative) or OISD Full (comprehensive).  
[oisd.nl](https://oisd.nl)

### StevenBlack
Classic combined hosts list. [github.com/StevenBlack/hosts](https://github.com/StevenBlack/hosts)

### My custom Microsoft and Google blocklist (inclute white list)

> [!CAUTION]
> I noticed that despite YouTube's whitelisting, the mobile apps were unresponsive and that requests to Google were blocked when connecting via a browser. Therefore, it's crucial to be very careful when adding this list to AdGuard Home or any other DNS-based service you might be using.

Will block all Microsoft and Google services except:
- GitHub / VS Code
- Microsoft Documentations 
- Windows Update
- Windows Activation
- Windows NTP server
- Login with Google
- YouTube
- Google images CDN
- Google DNS (DoH)

[google-msft-blocklist.txt](/08-dns-filtering/google-msft-blocklist.txt) to add into your DNS filter.

## Starting Recommendation
**Hagezi Multi Pro + OISD Full** as a baseline. Whitelist broken sites as needed.
