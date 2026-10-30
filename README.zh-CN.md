# Network Tools List

[English](README.md) | [Français](README.fr.md) | [Español](README.es.md) | **中文** | [日本語](README.ja.md) | [Русский](README.ru.md)

网络诊断与监控工具及命令

□ QQ 抓取和检查

命令/工具 {} 它会做什么?
|---|---|
通过端口过滤的 `tcpdump -i any -n port 443` Live 包抓取
`tshark -i en0 -Y dns` 配有显示过滤器的 Wireshark CLI QQ
`ngrep -q 'password'` 飞行时的Grep包
QQ [Snitch] (https://github.com/aixisstudio/Snitch) QUI: 每一个连接 ~ 进程, 国家, 在一个点击 ~ 中块

□ □ 发现

命令/工具 {} 它会做什么?
|---|---|
`nmap -sV -O 192.168.1.0/24` 服务 + OS 探测子网 QQ
`arp-scan -l` 列出局域网上的每个设备 {}
`mtr -n 8.8.8.8` 微量路线+ping 组合,直播 QQ
`ss -tulpn` 谁在听谁在说话?
`lsof -i -P -n` 过程 ~ 连接映射 ~

#####DNS #########################################################################################################################################################################################################################################################

{\fn华文楷体\fs16\1cHE0E0E0}命令 它会做什么?
|---|---|
`dig +short example.com` 快速A/AAA搜索QQ
`dig @1.1.1.1 example.com ANY` 查询特定解析器 QQ
`doggo example.com` 现代人类友好挖掘
`resolvectl flush-caches` 清除系统的 DNS 缓存 QQ

# # # # # 测量调试

命令/工具 {} 它会做什么?
|---|---|
`iperf3 -c server` 两个主机之间的通量 QQ
* `mtr`, `pathping` (Win) * * 路径的延迟/跳 * *
`bandwhich` 每进程带宽使用量
QQ `iftop` / `nethogs` – Live 接口/进程流量QQ
`curl -w '@timing.txt'` 请求暂时失效

##### 防火墙(每OS)

现场记录
|---|---|
Linux `nftables`, `iptables`, `firewalld`, `ufw`, eBPF QQ
(原始内容存档于2018-09-21). MACOS `pf`, LuLu (GUI) |.
Windows 粮食计划署(简易墙图形界面),`netsh advfirewall` QQ
BSD `pf`, `ipfw` | |

# # # # # 无线

* 工具 * * * 它会做什么?
|---|---|
`aircrack-ng`套房 抓捕、注射、审计 802.11 QQ
`Kismet` 被动无线IDS QQ
`wavemon` 终极无线信号显示器

# # # # 运行 & BGP

* 工具 * * 描述 * *
|---|---|
[BGPStream](https://bgpstream.caida.org/) QQLive BGP数据馈送 QQ
(https://atlas.ripe.net/) 全球探测网
[bgp.he.net](https://bgp.he.net/) 飓风BGP寻觅 腾讯网.
[PeeringDB] (https://www.peeringdb.com/) |. 与谁同行?
(https://github.com/FRRouting/frr) 开源路由套房

□ QQ 防火墙和过滤( extras)

* 工具 * * 描述 * *
|---|---|
|[pf](https://www.openbsd.org/faq/pf/)| OpenBSD的防火墙——最干净的|.
[表/nftables](https://netfilter.org/) | Linux本土过滤 |
[Gluetun](https://github.com/qdm12/gluetun) 整堆的 VPN 客户端容器 QQ

□ □ 包装工艺( extras)

* 工具 * * 描述 * *
|---|---|
[hping3](https://github.com/antirez/hping) | TCP/IP包装器 |
[Yersinia] (https://github.com/tomac/yersinia) QQ L2协议攻击 QQ
[包装](https://github.com/jemcek/packETH) \\\ \ \ \ \ \ 图形用户界面包构建器\ \

# # # # # 无线

* 工具 * * 描述 * *
|---|---|
(https://github.com/aircrack-ng/aircrack-ng)无线安全套房
[吻](https://www.kismetwireless.net/) | 无线探测器/嗅觉 |
[hcxdumptool] (https://github.com/ZerBea/hcxdumptool) 捕捉大麻猫...
[Bettercap](https://github.com/bettercap/bettercap) 瑞士军队MITM框架 QQ

---
## 贡献

欢迎提交 Pull Request，我们会审查并合并。由 [aixisstudio](https://github.com/aixisstudio) 维护，他也是开源应用防火墙 [Snitch](https://github.com/aixisstudio/Snitch) 的作者。

## 许可证: MIT
