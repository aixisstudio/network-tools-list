# Network Tools List

[English](README.md) | [Français](README.fr.md) | [Español](README.es.md) | [中文](README.zh-CN.md) | [日本語](README.ja.md) | **Русский**

Инструменты и команды диагностики сети

###Захват и проверка

Командный инструмент / Command Что он делает
|---|---|
| `tcpdump -i any -n port 443` | Захват пакетов в реальном времени фильтруется портом |
| `tshark -i en0 -Y dns` | Wireshark's CLI с фильтрами отображения |
| `ngrep -q 'password'` | пакеты grep, когда они летают
| [Snitch] (https://github.com/aixisstudio/Snitch) | GUI: каждое соединение → процесс, страна, блок в один клик |

##   Открытие

Командный инструмент / Command Что он делает
|---|---|
| `nmap -sV -O 192.168.1.0/24` | Обнаружение службы + ОС в подсети |
`arp-scan -l` Перечислите все устройства в локальной сети
| `mtr -n 8.8.8.8` | traceroute + ping Combined, live |
`ss -tulpn` Кто слушает и кто говорит (статистика сокетов)
| `lsof -i -P -n` | Процесс отображения соединения |

##   DNS

Командир! Что он делает
|---|---|
| `dig +short example.com` | Быстрый поиск A/AAAA
| `dig @1.1.1.1 example.com ANY` | Запрос конкретного решателя |
| `doggo example.com` | Современные дружественные к человеку раскопки
| `resolvectl flush-caches` | Очистить системный кэш DNS |

##  Measure Мера и отладка

Командный инструмент / Command Что он делает
|---|---|
| `iperf3 -c server` | Пропускная способность между двумя узлами |
| `mtr`, `pathping` (Win) | Задержка пути на прыжок |
| `bandwhich` | Использование полосы пропускания для каждого процесса |
| `iftop`/`nethogs` | Живой интерфейс/процессный трафик
| `curl -w '@timing.txt'` | Разбивка задержки по запросу |

## ) Firewalling (для ОС)

| OS | Stack
|---|---|
Linux, `nftables`, `iptables`, `firewalld`, `ufw`, eBPF
| macOS | `pf`, LuLu (GUI)
Windows | WFP (simplewall GUI), `netsh advfirewall`
BSD, `pf`, `ipfw`

##  ️ Wi-Fi

Инструмент Что он делает
|---|---|
| `aircrack-ng` suite | Захват, инъекция, аудит 802.11 |
`Kismet` Пассивная беспроводная IDS
| `wavemon` | Терминальный монитор сигналов Wi-Fi |

## out Маршрутизация и BGP

| Инструмент | Описание
|---|---|
[BGPStream] (https://bgpstream.caida.org/) | Live BGP data feed |
[RIPE Atlas] (https://atlas.ripe.net/) | Глобальная зондовая сеть
[bgp.he.net] (https://bgp.he.net/) | Ураган Электрический поиск BGP
[PeeringDB] (https://www.peeringdb.com/) Кто с кем дружит
| [FRRouting] (https://github.com/FRRouting/frr) | Комплект маршрутизации с открытым исходным кодом |

Firewall & Filtering (дополнение)

| Инструмент | Описание
|---|---|
[pf](https://www.openbsd.org/faq/pf/) | брандмауэр OpenBSD — самый чистый |
| [ebtables/nftables] (https://netfilter.org/) | Нативная фильтрация Linux
| [Gluetun] (https://github.com/qdm12/gluetun) | Контейнер клиента VPN для целых стеков |

## ) Пакетное ремесло (дополнительные)

| Инструмент | Описание
|---|---|
| [hping3](https://github.com/antirez/hping) | TCP/IP пакетный ассемблер |
[Yersinia] (https://github.com/tomac/yersinia) | Атаки протокола L2
| [пакет] (https://github.com/jemcek/packETH) | сборщик пакетов GUI |

##   Wi-Fi

| Инструмент | Описание
|---|---|
| [aircrack-ng] (https://github.com/aircrack-ng/aircrack-ng) | Комплект безопасности Wi-Fi |
[Kismet] (https://www.kismetwireless.net/) | Беспроводной детектор / сниффер
[hcxdumptool] (https://github.com/ZerBea/hcxdumptool) | Захват для хэшката |
[Bettercap] (https://github.com/bettercap/bettercap) | Структура MITM швейцарской армии

---
## Участие

Pull request'ы приветствуются — открой PR, он будет проверен и принят. Ведёт [aixisstudio](https://github.com/aixisstudio), автор [Snitch](https://github.com/aixisstudio/Snitch) — open-source application firewall.

## Лицензия: MIT
