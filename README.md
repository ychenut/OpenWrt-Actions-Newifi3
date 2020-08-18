# OpenWrt firmware for Newifi D2

Auto build OpenWrt firmware for Newifi D2 via GitHub Actions

[![GitHub release (latest by date)](https://img.shields.io/github/v/release/P3TERX/OpenWrt-Newifi_D2?style=for-the-badge&label=Download)](https://github.com/ZHDeveloper/OpenWrt-Newifi_D2/actions/)

### 开原驱动配置

```
CONFIG_PACKAGE_kmod-mt7603=y
CONFIG_PACKAGE_kmod-mt7603e=n
CONFIG_PACKAGE_kmod-mt76x2=y
CONFIG_PACKAGE_kmod-mt76x2-common=y
CONFIG_PACKAGE_kmod-mt76x2e=n
CONFIG_PACKAGE_wpad-openssl=y
CONFIG_PACKAGE_wpa-supplicant=y

CONFIG_PACKAGE_luci-app-mtwifi=n
```

### LuCI应用说明
- luci-app-accesscontrol #访问时间控制
- luci-app-adbyby-plus #广告屏蔽大师Plus +
- luci-app-arpbind #IP/MAC绑定
- luci-app-autoreboot #支持计划重启
- luci-app-ddns #动态域名 DNS（集成阿里DDNS客户端）
- luci-app-filetransfer #文件传输（可web安装ipk包）
- luci-app-firewall #添加防火墙
- luci-app-flowoffload #Turbo ACC网络加速（集成FLOW,BBR,NAT,DNS...
- luci-app-frpc #内网穿透 Frp
- luci-app-guest-wifi #WiFi访客网络
- luci-app-mwan3 #MWAN3负载均衡
- luci-app-mwan3helper #MWAN3分流助手
- luci-app-nlbwmon #网络带宽监视器
- luci-app-ramfree #释放内存
- luci-app-samba #网络共享（Samba）
- luci-app-sqm #流量智能队列管理（QOS）
- luci-app-syncdial #多拨虚拟网卡（原macvlan）
- luci-app-unblockmusic #解锁网易云灰色歌曲
- luci-app-upnp #通用即插即用UPnP（端口自动转发）
- luci-app-vlmcsd #KMS服务器设置
- luci-app-vsftpd #FTP服务器
- luci-app-wifischedule #WiFi 计划
- luci-app-wol #WOL网络唤醒
- luci-app-wrtbwmon #实时流量监测
- luci-app-xlnetacc #迅雷快鸟
- luci-app-zerotier #ZeroTier内网穿透

--

- luci-app-accesscontrol #访问时间控制
- luci-app-acme #ACME 自动化证书管理环境
- luci-app-adblock #ADB广告过滤
- luci-app-adbyby-plus #广告屏蔽大师Plus +
- luci-app-adbyby #广告过滤大师（已弃）
- luci-app-adkill #广告过滤（已弃）
- luci-app-advanced-reboot #Linksys高级重启
- luci-app-ahcp #支持AHCPd
- luci-app-aliddns #阿里DDNS客户端（已弃，集成至ddns）
- luci-app-amule #aMule下载工具
- luci-app-aria2 # Aria2下载工具
- luci-app-arpbind #IP/MAC绑定
- luci-app-asterisk #支持Asterisk电话服务器
- luci-app-attendedsysupgrade #固件更新升级相关
- luci-app-autoreboot #支持计划重启
- luci-app-baidupcs-web #百度网盘管理 *
- luci-app-bcp38 #BCP38网络入口过滤（不确定）
- luci-app-bird1-ipv4 #对Bird1-ipv4的支持
- luci-app-bird1-ipv6 #对Bird1-ipv6的支持
- luci-app-bird4 #Bird 4（未知）（已弃）
- luci-app-bird6 #Bird 6（未知）（已弃）
- luci-app-bmx6 #BMX6路由协议
- luci-app-bmx7 #BMX7路由协议
- luci-app-caldav #联系人（已弃）
- luci-app-cifsd #网络共享CIFS/SMB服务器 *
- luci-app-cjdns #加密IPV6网络相关
- luci-app-clamav #ClamAV杀毒软件
- luci-app-commands #Shell命令模块
- luci-app-cshark #CloudShark捕获工具
- luci-app-ddns #动态域名 DNS（集成阿里DDNS客户端）
- luci-app-diag-core #core诊断工具
- luci-app-dnscrypt-proxy #DNSCrypt解决DNS污染
- luci-app-dnsforwarder #DNSForwarder防DNS污染
- luci-app-dnspod #DNSPod动态域名解析
- luci-app-dockerman #Docker容器 *
- luci-app-dump1090 #民航无线频率（不确定）
- luci-app-dynapoint #DynaPoint（未知）
- luci-app-e2guardian #Web内容过滤器
- luci-app-familycloud #家庭云盘
- luci-app-filetransfer #文件传输（可web安装ipk包）
- luci-app-firewall #添加防火墙
- luci-app-flowoffload #Turbo ACC网络加速（集成FLOW,BBR,NAT,DNS...
- luci-app-freifunk-diagnostics #freifunk组件 诊断（未知）
- luci-app-freifunk-policyrouting #freifunk组件 策略路由（未知）
- luci-app-freifunk-widgets #freifunk组件 索引（未知）
- luci-app-frpc #内网穿透 Frp
- luci-app-fwknopd #Firewall Knock Operator服务器
- luci-app-guest-wifi #WiFi访客网络
- luci-app-haproxy-tcp #HAProxy负载均衡-TCP
- luci-app-hd-idle #硬盘休眠
- luci-app-hnet #Homenet Status家庭网络控制协议
- luci-app-ipsec-virtuald #virtual服务器 IPSec
- luci-app-kodexplorer #KOD可道云私人网盘
- luci-app-kooldns #virtual**服务器 ddns替代方案（已弃）
- luci-app-koolproxy #KP去广告（已弃）
- luci-app-lxc #LXC容器管理
- luci-app-meshwizard #网络设置向导
- luci-app-minidlna #完全兼容DLNA / UPnP-AV客户端的服务器软件
- luci-app-mjpg-streamer #兼容Linux-UVC的摄像头程序
- luci-app-mtwifi #MTWiFi驱动的支持 *
- luci-app-mmc-over-gpio #添加SD卡操作界面（已弃）
- luci-app-multiwan #多拨虚拟网卡（已弃，移至syncdial）
- luci-app-mwan #MWAN负载均衡（已弃）
- luci-app-mwan3 #MWAN3负载均衡
- luci-app-mwan3helper #MWAN3分流助手
- luci-app-n2n_v2 #N2N内网穿透 N2N v2 virtual**服务
- luci-app-netdata #Netdata实时监控（图表） *
- luci-app-nft-qos #QOS流控 Nftables版
- luci-app-ngrokc #Ngrok 内网穿透（已弃）
- luci-app-nlbwmon #网络带宽监视器
- luci-app-noddos #NodDOS Clients 阻止DDoS攻击
- luci-app-nps #内网穿透nps *
- luci-app-ntpc #NTP时间同步服务器
- luci-app-olsr #OLSR配置和状态模块
- luci-app-olsr-services #OLSR服务器
- luci-app-olsr-viz #OLSR可视化
- luci-app-oscam #OSCAM服务器（已弃）
- luci-app-p910nd #打印服务器模块
- luci-app-pagekitec #Pagekite内网穿透客户端
- luci-app-polipo #Polipo代理(是一个小型且快速的网页缓存代理)
- luci-app-pppoe-relay #PPPoE NAT穿透 点对点协议（PPP）
- luci-app-privoxy #Privoxy网络代理(带过滤无缓存)
- luci-app-qbittorrent #BT下载工具（qBittorrent）
- luci-app-qos #流量服务质量(QoS)流控
- luci-app-radicale #CalDAV/CardDAV同步工具
- luci-app-ramfree #释放内存
- luci-app-rp-pppoe-server #Roaring Penguin PPPoE Server 服务器
- luci-app-samba #网络共享（Samba）
- luci-app-samba4 #网络共享（Samba4）
- luci-app-sfe #Turbo ACC网络加速（flowoffload二选一）
- luci-app-shairplay #支持AirPlay功能
- luci-app-siitwizard #SIIT配置向导 SIIT-Wizzard
- luci-app-simple-adblock #简单的广告拦截
- luci-app-smartdns #SmartDNS本地服务器 *
- luci-app-splash #Client-Splash是无线MESH网络的一个热点认证系统
- luci-app-sqm #流量智能队列管理（QOS）
- luci-app-squid #Squid代理服务器
- luci-app-statistics #流量监控工具
- luci-app-syncdial #多拨虚拟网卡（原macvlan）
- luci-app-tinyproxy #Tinyproxy是 HTTP(S)代理服务器
- luci-app-transmission #BT下载工具
- luci-app-travelmate #旅行路由器
- luci-app-ttyd #网页终端命令行
- luci-app-udpxy #udpxy做组播服务器
- luci-app-uhttpd #uHTTPd Web服务器
- luci-app-unblockmusic #解锁网易云灰色歌曲
- luci-app-unblockneteasemusic-go #解锁网易云歌曲 *
- luci-app-unbound #Unbound DNS解析器
- luci-app-upnp #通用即插即用UPnP（端口自动转发）
- luci-app-usb-printer #USB 打印服务器
- luci-app-verysync #微力同步 *
- luci-app-vlmcsd #KMS服务器设置
- luci-app-vnstat #vnStat网络监控（图表）
- luci-app-vsftpd #FTP服务器
- luci-app-watchcat #断网检测功能与定时重启
- luci-app-webadmin #Web管理页面设置
- luci-app-webshell #网页命令行终端（已弃）
- luci-app-wifischedule #WiFi 计划
- luci-app-wireguard #virtual**服务器 WireGuard状态
- luci-app-wol #WOL网络唤醒
- luci-app-wrtbwmon #实时流量监测
- luci-app-xlnetacc #迅雷快鸟
- luci-app-zerotier #ZeroTier内网穿透
