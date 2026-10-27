# Network Tools List

**English** | [Français](README.fr.md) | [Español](README.es.md) | [中文](README.zh-CN.md) | [日本語](README.ja.md) | [Русский](README.ru.md)

Network diagnostic & monitoring tools and commands

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

## 🧭 Routing & BGP

| Tool | Description |
|---|---|
| [BGPStream](https://bgpstream.caida.org/) | Live BGP data feed |
| [RIPE Atlas](https://atlas.ripe.net/) | Global probe network |
| [bgp.he.net](https://bgp.he.net/) | Hurricane Electric BGP lookup |
| [PeeringDB](https://www.peeringdb.com/) | Who peers with whom |
| [FRRouting](https://github.com/FRRouting/frr) | Open-source routing suite |

## 🔥 Firewall & Filtering (extras)

| Tool | Description |
|---|---|
| [pf](https://www.openbsd.org/faq/pf/) | OpenBSD's firewall — the cleanest |
| [ebtables/nftables](https://netfilter.org/) | Linux native filtering |
| [Gluetun](https://github.com/qdm12/gluetun) | VPN client container for whole stacks |

## 🧬 Packet Crafting (extras)

| Tool | Description |
|---|---|
| [hping3](https://github.com/antirez/hping) | TCP/IP packet assembler |
| [Yersinia](https://github.com/tomac/yersinia) | L2 protocol attacks |
| [packeth](https://github.com/jemcek/packETH) | GUI packet builder |

## 📶 Wi-Fi

| Tool | Description |
|---|---|
| [aircrack-ng](https://github.com/aircrack-ng/aircrack-ng) | Wi-Fi security suite |
| [Kismet](https://www.kismetwireless.net/) | Wireless detector/sniffer |
| [hcxdumptool](https://github.com/ZerBea/hcxdumptool) | Capture for hashcat |
| [Bettercap](https://github.com/bettercap/bettercap) | The Swiss-army MITM framework |

---
Maintained by [aixisstudio](https://github.com/aixisstudio) — author of [Snitch](https://github.com/aixisstudio/Snitch), the open-source application firewall.

## License

MIT
