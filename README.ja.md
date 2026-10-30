# Network Tools List

[English](README.md) | [Français](README.fr.md) | [Español](README.es.md) | [中文](README.zh-CN.md) | **日本語** | [Русский](README.ru.md)

ネットワーク診断・監視ツールとコマンド

## タスクとインスペクト

| コマンド・ツール | お問い合わせ |
|---|---|
| `tcpdump -i any -n port 443` | ポート別ライブパケットキャプチャ |
| `tshark -i en0 -Y dns` | ディスプレイフィルタ付きWiresharkのCLI |
| `ngrep -q 'password'` | 飛翔したパケット |
| [Snitch](https://github.com/aixisstudio/Snitch) | GUI: あらゆる接続 → プロセス、国、ワンクリックでブロック |

## ✓ 発見

| コマンド・ツール | お問い合わせ |
|---|---|
| `nmap -sV -O 192.168.1.0/24` | サービス + サブネットでのOS検出 |
| `arp-scan -l` | LAN全てのデバイスを一覧表示 |
| `mtr -n 8.8.8.8` | トレースルート + ping 組み合わせてライブ |
| `ss -tulpn` | 誰が聞き、誰が話しているのか(ソケットスタット) |
| `lsof -i -P -n` | プロセス → 接続マッピング |

## インポート DNS

| コマンド | お問い合わせ |
|---|---|
| `dig +short example.com` | クイック A/AAAAAA 外観 |
| `dig @1.1.1.1 example.com ANY` | 特定のリゾルバーの問い合わせ |
| `doggo example.com` | 現代人間に優しいディグ |
| `resolvectl flush-caches` | DNSキャッシュをクリア |

## 測定とデバッグ

| コマンド・ツール | お問い合わせ |
|---|---|
| `iperf3 -c server` | 2つのホスト間のスループット |
| `mtr`, `pathping`(Win) | ホップ当たりの通行止め |
| `bandwhich` | 加工帯域幅使用量 |
| `iftop` / `nethogs` | ライブインターフェース・加工トラフィック |
| `curl -w '@timing.txt'` | 課題解決事例 |

## ◀ ファイアウォール (OSごとに)

| OS | スタック |
|---|---|
| Linux | `nftables`、`iptables`、`firewalld`、`ufw`、eBPF |
| macOS | `pf`, ルル(GUI) |
| Windows | WFP(簡易壁GUI)、`netsh advfirewall` |
| `pf`, `ipfw` | `pf`, `ipfw` | `pf`, `ipfw` | `pf`, `ipfw`, `ipfw`, `ipfw`, `ipfw`, `pf`, `pf`, `ipfw`, `ipfw`, `ipfw`, `ipfw`, `ipfw`, `ipfw`, `ipfw`, `pf`, `pf`, `pf`, `pf`, `ipfw`, `ipfw`, `ipfw`, `ipfw`, `pf`, `pf`, `pf`, `pf`, `pf`, `pf`, `pf`, `pf`, `pf`, `pf`, `pf`, `pf`, `pf`, `pf`, `ipfw`, `pf`, `ipfw`, `pf`, `ipfw`, `pf`, `ipfw`, `ipfw`, `ipfw`,

## ️️ Wi-Fi

| ツール | お問い合わせ |
|---|---|
| `aircrack-ng` スイート | キャプチャ、インジェクト、監査 802.11 |
| `Kismet` | パッシブワイヤレスIDS |
| `wavemon` | ターミナルWi-Fi信号モニター |

## 🧭 ルーティング&BGP

| ツール | 説明 |
|---|---|
| 【BGPStream】(https://bgpstream.caida.org/) | ライブBGPデータフィード |
| 【RIPEアトラス】(https://atlas.ripe.net/) | グローバルプローブネットワーク |
| [bgp.he.net](https://bgp.he.net/) | ハリケーンエレクトリックBGPルックアップ |
| 【ペリングDB】(https://www.peeringdb.com/) | 誰とのか |
| 【FRRouting】(https://github.com/FRRouting/frr) | オープンソースルーティングスイート |

## ◀ ファイアウォールとフィルタリング (extras)

| ツール | 説明 |
|---|---|
| [pf](https://www.openbsd.org/faq/pf/) | OpenBSDのファイアウォール — 一番クリーンな |
| 【表紙・nftables】(https://netfilter.org/) | Linux ネイティブフィルタ |
|【Gluetun】(https://github.com/qdm12/gluetun) | 全スタック向けVPNクライアントコンテナ |

## 🧬 パケットクラフト (extras)

| ツール | 説明 |
|---|---|
| 【hping3】(https://github.com/antirez/hping) | TCP/IPパケットアセンブラ |
| [Yersinia](https://github.com/tomac/yersinia) | L2 プロトコル攻撃 |
| [packeth](https://github.com/jemcek/packETH) | GUIパケットビルダー |

## 📶 Wi-Fi

| ツール | 説明 |
|---|---|
| 【aircrack-ng】(https://github.com/aircrack-ng/aircrack-ng) | Wi-Fiセキュリティスイート |
| 【Kismet】(https://www.kismetwireless.net/) | ワイヤレスディテクタ・スニッファ |
| [hcxdumptool](https://github.com/ZerBea/hcxdumptool) | ハッシュキャットのキャプチャ |
| 【Bettercap】(https://github.com/bettercap/bettercap) | スイス・アーミーMITMフレームワーク |

---
## 貢献

プルリクエストを歓迎します。レビューしてマージします。[aixisstudio](https://github.com/aixisstudio) による管理 — オープンソースのアプリケーションファイアウォール [Snitch](https://github.com/aixisstudio/Snitch) の作者です。

## ライセンス: MIT
