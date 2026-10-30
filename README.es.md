# Network Tools List

[English](README.md) | [Français](README.fr.md) | **Español** | [中文](README.zh-CN.md) | [日本語](README.ja.md) | [Русский](README.ru.md)

Herramientas y comandos de diagnóstico de red

## 📡 Capture &amp; Inspect

Mando / Herramienta permanente Lo que hace
|---|---|
Silencio `tcpdump -i any -n port 443` Silencio Captura de paquete en vivo filtrado por port Silencio
CLI de Wireshark con filtros de pantalla Silencio
Silencio `ngrep -q 'password'` Silencioso paquetes de grep mientras vuelan por
Silencio [Snitch] (https://github.com/aixisstudio/Snitch) Silencio GUI: cada conexión → proceso, país, bloque en un solo clic

Descubrir

Mando / Herramienta permanente Lo que hace
|---|---|
← `nmap -sV -O 192.168.1.0/24` Silencioso Servicio + Detección del sistema operativo en una subnet
← `arp-scan -l` Silencio Listar todos los dispositivos en la LAN
Silencio `mtr -n 8.8.8.8` Silencioso trazador + ping combinado, vivo
Silencio `ss -tulpn` Silencio ¿Quién está escuchando?
Silencio `lsof -i -P -n` Silencio Proceso → cartografía de la conexión

## 🌐 DNS

Silencio Lo que hace
|---|---|
Silencio `dig +short example.com` Silencio Quick A/AAAA lookup
Silencio `dig @1.1.1.1 example.com ANY` Silencio Query a specific resolve Silencio
Silencio `doggo example.com`
Silencio `resolvectl flush-caches` Silencio Limpiar el sistema DNS cache ANTE

## 📊 Measure &gt; Debug

Mando / Herramienta permanente Lo que hace
|---|---|
Silencio `iperf3 -c server` TENIDO A través de la comunicación entre dos anfitriones
← `mtr`, `pathping` (Win)
Silencio `bandwhich` Silencio Uso de ancho de banda por proceso
← `iftop` / `nethogs`
Silencio `curl -w '@timing.txt'`

## 🔥 Firewalling (per OS)

Silencioso sistema operativo
|---|---|
TEN Linux ANTE `nftables`, `iptables`, `firewalld`, `ufw`, eBPF ANTE
TENIDO macOS TENIDO `pf`, LuLu (GUI)
← Windows ← PMA (simplewall GUI), `netsh advfirewall`
← BSD   `pf`, `ipfw`

Wi-Fi

← Herramienta permanente Lo que hace
|---|---|
← `aircrack-ng` suite ¦ Capture, inyect, auditar 802.11
Silencio `Kismet`
Silencio `wavemon` Silencio Terminal Monitor de señal Wi-Fi Silencio

## 🧭 Routing &gt; BGP

← Herramienta Silencioso
|---|---|
Silencio [BGPStream] (https://bgpstream.caida.org/)
confidencialidad [RIPE Atlas] (https://atlas.ripe.net/)
[bgp.he.net] (https://bgp.he.net/)
[PeeringDB] (https://www.peeringdb.com/) ¿Quiénes son los compañeros con quienes vivieron?
Silencio [FRRouting] (https://github.com/FRRouting/frr)

## 🔥 Firewall &amp; Filtering (extras)

← Herramienta Silencioso
|---|---|
Silencio [pf] (https://www.openbsd.org/faq/pf/)
(https://netfilter.org/)
[Gluetun] (https://github.com/qdm12/gluetun) Silencioso VPN cliente contenedor para pilas enteras

## 🧬 Packet Crafting (extras)

← Herramienta Silencioso
|---|---|
[hping3] (https://github.com/antirez/hping)
Silencio [Yersinia] (https://github.com/tomac/yersinia)
[paquete] (https://github.com/jemcek/packETH)

## 📶 Wi-Fi

← Herramienta Silencioso
|---|---|
Silencio [aircrack-ng] (https://github.com/aircrack-ng/aircrack-ng)
Silencio [Kismet] (https://www.kismetwireless.net/)
[hcxdumptool] (https://github.com/ZerBea/hcxdumptool)
Silencio [Bettercap] (https://github.com/bettercap/bettercap)

---
## Contribuir

Los pull requests son bienvenidos: abre una PR y será revisada y fusionada. Mantenido por [aixisstudio](https://github.com/aixisstudio), autor de [Snitch](https://github.com/aixisstudio/Snitch), firewall de aplicaciones open source.

## Licencia: MIT
