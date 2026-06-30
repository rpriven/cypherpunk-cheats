# Cypherpunk Cheats

Navi-compatible cheatsheets for security, privacy, and digital sovereignty.

50 cheatsheets spanning offensive security, DFIR, privacy, encryption, system hardening, and cryptocurrency.

## Installation

```bash
# Install navi
cargo install navi
# or: sudo apt install navi   (Debian/Ubuntu)   |   brew install navi   (macOS)

# Add this repo to navi (choose one)
navi repo add https://github.com/rpriven/cypherpunk-cheats        # GitHub
navi repo add https://git.djeditech.com/djedi/cypherpunk-cheats   # Mirror
```

## Manual Setup

Point navi at a local clone (best for editing/dogfooding) — `~/.config/navi/config.yaml`:

```yaml
cheats:
  paths:
    - /path/to/cypherpunk-cheats
```

## Usage

```bash
navi                          # interactive launcher
navi --query "ufw"            # jump to a topic
navi --best-match --query "ssh hardening" --print   # print top match, no TUI
```

## Categories

### Offensive Security & Recon
| File | Description |
|------|-------------|
| `nmap.cheat` | Port scanning and service enumeration |
| `recon-advanced.cheat` | Advanced recon / OSINT enumeration |
| `web.cheat` | Web app testing (Burp, ffuf, fuzzing) |
| `api-testing.cheat` | REST/GraphQL API testing |
| `vuln-scanning.cheat` | Vulnerability scanning |
| `hashcat.cheat` | Password cracking with Hashcat |
| `john.cheat` | John the Ripper password cracking |
| `privesc-linux.cheat` | Linux privilege escalation |
| `privesc-windows.cheat` | Windows privilege escalation |
| `active-directory.cheat` | AD attacks (Kerberos, NetExec) |
| `ad-post-exploit.cheat` | AD post-exploitation / lateral movement |
| `smb-shares.cheat` | SMB shares & lateral movement |
| `c2-frameworks.cheat` | Command-and-control frameworks |
| `wireless.cheat` | WiFi attacks (aircrack-ng, WPA) |
| `tunnels.cheat` | SSH tunnels, pivoting, port-forward, WireGuard |
| `containers.cheat` | Docker/Kubernetes security & escapes |
| `reversing.cheat` | Ghidra, radare2, GDB, binary analysis |

### DFIR & Analysis
| File | Description |
|------|-------------|
| `forensics.cheat` | Volatility, memory, incident response |
| `wireshark.cheat` | Packet analysis (tshark, tcpdump) |
| `osint.cheat` | Sherlock, theHarvester, recon-ng |
| `steganography.cheat` | Hidden data (steghide, binwalk) |

### Privacy & Anonymity
| File | Description |
|------|-------------|
| `privacy.cheat` | Privacy toolkit overview (Tor, GPG, PETs) |
| `tor.cheat` | Tor, onion services, darknet |
| `anti-surveillance.cheat` | Counter-surveillance & tracking defense |
| `browser-hardening.cheat` | Firefox/Chrome hardening, anti-fingerprinting |
| `phone-privacy.cheat` | Mobile privacy (GrapheneOS, Android, iOS) |
| `metadata-removal.cheat` | EXIF / metadata sanitization |
| `opsec.cheat` | Operational security & threat modeling |
| `secure-comms.cheat` | Signal, Matrix, SimpleX, encrypted messaging |
| `email-privacy.cheat` | ProtonMail/Tutanota, PGP email |

### Encryption & Secrets
| File | Description |
|------|-------------|
| `gpg.cheat` | GPG/PGP encryption & signing |
| `age.cheat` | Modern file encryption (age) |
| `luks.cheat` | Full-disk encryption (LUKS, dm-crypt) |
| `veracrypt.cheat` | VeraCrypt containers & hidden volumes |
| `pass.cheat` | Password managers (pass, KeePassXC) |
| `2fa-security.cheat` | TOTP, FIDO2, YubiKey, MFA |
| `secure-file-sharing.cheat` | OnionShare, magic-wormhole |
| `secure-deletion.cheat` | Secure wipe (shred, data destruction) |
| `anti-forensics.cheat` | Counter-forensics / evidence elimination |

### System Hardening
| File | Description |
|------|-------------|
| `secure-os.cheat` | Tails, Whonix, Qubes, hardened Linux |
| `sandboxing.cheat` | firejail, bubblewrap, Flatpak/Flatseal, distrobox |
| `firewall.cheat` | ufw, nftables, iptables (Tailscale-safe) |
| `ssh-hardening.cheat` | sshd hardening, keys-only, modern crypto |
| `dns-privacy.cheat` | DoH/DoT, dnscrypt, unbound, Pi-hole |

### Cryptocurrency & Web3
| File | Description |
|------|-------------|
| `monero.cheat` | Monero CLI wallet operations |
| `monero-wallet-cli.cheat` | Monero wallet: keys, addresses, transfers, tx proofs |
| `bitcoin.cheat` | Bitcoin Core CLI operations |
| `anonymous-payments.cheat` | Private payments (Monero, Lightning, cash) |
| `solidity.cheat` | Smart-contract auditing (Slither, Foundry) |
| `nak.cheat` | Nostr army knife (fiatjaf's `nak`) |

## Philosophy

Built for cypherpunks who value:
- **Privacy** — default to encrypted, anonymous, and sovereign
- **Security** — offensive knowledge for defensive thinking
- **Freedom** — tools for digital self-determination

## Contributing

PRs welcome. Follow the navi `.cheat` format:
- `%` tags for categories
- `#` comments for descriptions
- `$` for argument completion

Use placeholders (`<var>`), never real keys, IPs, or addresses.

## License

MIT
