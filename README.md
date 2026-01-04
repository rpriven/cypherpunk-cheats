# Cypherpunk Cheats

Navi-compatible cheatsheets for security, privacy, and digital sovereignty.

## Installation

```bash
# Install navi
cargo install navi

# Or via package manager
sudo apt install navi  # Debian/Ubuntu
brew install navi      # macOS

# Add this repo to navi (choose one)
navi repo add https://github.com/rpriven/cypherpunk-cheats        # GitHub
navi repo add https://git.djeditech.com/djedi/cypherpunk-cheats   # Mirror
```

## Manual Setup

Add to your navi config (`~/.config/navi/config.yaml`):

```yaml
cheats:
  paths:
    - /path/to/cypherpunk-cheats
```

## Usage

```bash
# Launch navi
navi

# Query specific topic
navi --query "nmap"
navi --query "monero"
navi --query "luks"

# Preview mode
navi --preview

# Use with custom path
navi --path /path/to/cypherpunk-cheats
```

## Categories

### Offensive Security
| File | Description |
|------|-------------|
| `nmap.cheat` | Port scanning and service enumeration |
| `web.cheat` | Web application testing (ffuf, sqlmap, nikto) |
| `hashcat.cheat` | Password cracking with Hashcat |
| `john.cheat` | John the Ripper password cracking |
| `privesc-linux.cheat` | Linux privilege escalation |
| `privesc-windows.cheat` | Windows privilege escalation |
| `active-directory.cheat` | AD attacks (NetExec, Kerberoasting) |
| `containers.cheat` | Docker/Kubernetes security |
| `wireless.cheat` | WiFi attacks (aircrack-ng, WPA cracking) |
| `tunnels.cheat` | SSH tunnels, chisel, pivoting |

### DFIR & Analysis
| File | Description |
|------|-------------|
| `forensics.cheat` | Volatility, disk imaging, evidence collection |
| `osint.cheat` | Sherlock, theHarvester, recon-ng |
| `wireshark.cheat` | Packet analysis (tshark, tcpdump) |
| `reversing.cheat` | Ghidra, radare2, GDB, binary analysis |
| `steganography.cheat` | Hidden data extraction (steghide, binwalk) |

### Privacy & Encryption
| File | Description |
|------|-------------|
| `privacy.cheat` | Tor, GPG, age encryption, metadata removal |
| `luks.cheat` | Full disk encryption (LUKS, dm-crypt) |
| `pass.cheat` | Password managers (pass, KeePassXC) |
| `secure-comms.cheat` | Signal CLI, Matrix, encrypted messaging |

### Cryptocurrency & Web3
| File | Description |
|------|-------------|
| `monero.cheat` | Monero CLI wallet operations |
| `bitcoin.cheat` | Bitcoin Core CLI operations |
| `solidity.cheat` | Smart contract auditing (Slither, Foundry) |

## Philosophy

Built for cypherpunks who value:
- **Privacy** - Default to encrypted, anonymous, and sovereign
- **Security** - Offensive knowledge for defensive thinking
- **Freedom** - Tools for digital self-determination

## Contributing

PRs welcome! Follow the navi `.cheat` format:
- `%` tags for categories
- `#` comments for descriptions
- `$` for argument completion

## License

MIT
