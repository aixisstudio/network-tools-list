# Network Tools List

[English](README.md) | **Français** | [Español](README.es.md) | [中文](README.zh-CN.md) | [日本語](README.ja.md) | [Русский](README.ru.md)

Outils et commandes de diagnostic et monitoring réseau

Capture et inspection

Commande / Outil Ce qu'il fait
|---|---|
`tcpdump -i any -n port 443`: capture de paquets en direct filtrée par le port
CLI de Wireshark avec filtres d'affichage
Les paquets de grep `ngrep -q 'password'`
[Snitch](https://github.com/aixisstudio/Snitch)=GUI: chaque connexion → processus, pays, bloquer en un seul clic=

Découvrir

Commande / Outil Ce qu'il fait
|---|---|
Service + détection d'OS sur un sous-réseau
`arp-scan -l`. Lister tous les appareils sur le LAN.
`mtr -n 8.8.8.8`=Ligneroute + ping combiné, live=
Qui écoute et qui parle (statistiques de poche)
Processus de `lsof -i -P -n`

DNS

Commandement Ce qu'il fait
|---|---|
Recherche rapide A/AAAA
`dig @1.1.1.1 example.com ANY`: Interroger un résolveur spécifique
`doggo example.com`
Effacer le cache DNS systemd

Mesure et débogage

Commande / Outil Ce qu'il fait
|---|---|
`iperf3 -c server`=Traitement entre deux hôtes
Latence par houblon
Utilisation de la bande passante par processus
`iftop` / `nethogs`
`curl -w '@timing.txt'`

Pare-feu (par OS)

O.S. Empilement
|---|---|
Linux, `nftables`, `iptables`, `firewalld`, `ufw`, eBPF
`pf`, LuLu (GUI)
Fenêtres du PAM (interface graphique simple), `netsh advfirewall`
CdPH0X, CdPH1X

Wi-Fi

Outil Ce qu'il fait
|---|---|
Capturer, injecter, vérifier 802.11
IDS sans fil passif
`wavemon`-L'écran de signal Wi-Fi terminal

Routage et BGP

Description de l'outil
|---|---|
[BGPStream](https://bgpstream.caida.org/) (Feed de données BGP en direct)
Réseau de sonde mondial
[bgp.he.net](https://bgp.he.net/)
[PeeringDB] (https://www.peeringdb.com/) Avec qui?
[FRRouting](https://github.com/FRRouting/frr)

Pare-feu et filtrage (extras)

Description de l'outil
|---|---|
Le pare-feu d'OpenBSD — le plus propre
[Ebtables/nftables](https://netfilter.org/)
[Gluetun](https://github.com/qdm12/gluetun)

Fabrication de paquets (extras)

Description de l'outil
|---|---|
[hping3] (https://github.com/antirez/hping)
[Yersinia] (https://github.com/tomac/yersinia)
[packeth](https://github.com/jemcek/packETH)

Wi-Fi

Description de l'outil
|---|---|
Suite de sécurité Wi-Fi
[Kismet] (https://www.kismetwireless.net/)
[hcxdumptool](https://github.com/ZerBea/hcxdumptool)= Capture pour le haschcat=
[Bettercap] (https://github.com/bettercap/bettercap)Le cadre MITM Swiss-army

---
## Contribuer

Les pull requests sont les bienvenues : ouvre une PR, elle sera relue et fusionnée. Maintenu par [aixisstudio](https://github.com/aixisstudio), auteur de [Snitch](https://github.com/aixisstudio/Snitch), pare-feu applicatif open source.

## Licence: MIT
