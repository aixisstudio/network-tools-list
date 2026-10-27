# Network Tools List

[English](README.md) | **Français** | [Español](README.es.md) | [中文](README.zh-CN.md) | [日本語](README.ja.md) | [Русский](README.ru.md)

Outils et commandes de diagnostic et monitoring réseau

_Le contenu détaillé (listes, liens, descriptions) est en anglais pour rester maintenable — les sections ci-dessous te guident._

## 📡 Capture & Inspect

| Command / Tool | What it does |
|---|---|
| `tcpdump -i any -n port 443` | Live packet capture filtered by port |
| `tshark -i en0 -Y dns` | Wireshark's CLI with display filters |
| `ngrep -q 'password'` | grep packets as they fly by |
| [Snitch](https://github.com/aixisstudio/Snitch) | GUI: every connection → process, country, block in one click |

## 🔎 Discover

| Command / Tool | What it does |
|---|---|
| `nmap -sV -O 192.168.1.0/24` | Service + OS detection on a subnet |
| `arp-scan -l` | List every device on the LAN |
| `mtr -n 8.8.8.8` | traceroute + ping combined, live |
| `ss -tulpn` | Who's listening & who's talking (socket stats) |
| `lsof -i -P -n` | Process → connection mapping |

## 🌐 DNS

| Command | What it does |
|---|---|
| `dig +short example.com` | Quick A/AAAA lookup |
| `dig @1.1.1.1 example.com ANY` | Query a specific resolver |
| `doggo example.com` | Modern human-friendly dig |
| `resolvectl flush-caches` | Clear the systemd DNS cache |

## 📊 Measure & Debug

| Command / Tool | What it does |
|---|---|
| `iperf3 -c server` | Throughput between two hosts |
| `mtr`, `pathping` (Win) | Path latency per hop |
| `bandwhich` | Per-process bandwidth usage |
| `iftop` / `nethogs` | Live interface/process traffic |
| `curl -w '@timing.txt'` | Per-request latency breakdown |

## 🔥 Firewalling (per OS)

| OS | Stack |
|---|---|
| Linux | `nftables`, `iptables`, `firewalld`, `ufw`, eBPF |
| macOS | `pf`, LuLu (GUI) |
| Windows | WFP (simplewall GUI), `netsh advfirewall` |
| BSD | `pf`, `ipfw` |

## 🛰️ Wi-Fi

| Tool | What it does |
|---|---|
| `aircrack-ng` suite | Capture, inject, audit 802.11 |
| `Kismet` | Passive wireless IDS |
| `wavemon` | Terminal Wi-Fi signal monitor |

---
## Contribuer

Les pull requests sont les bienvenues : ouvre une PR, elle sera relue et fusionnée. Maintenu par [aixisstudio](https://github.com/aixisstudio), auteur de [Snitch](https://github.com/aixisstudio/Snitch), pare-feu applicatif open source.

## Licence: MIT
