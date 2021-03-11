# 简介

本项目生成适用于 [**Surge**](https://nssurge.com) 的规则集（DOMAIN-SET 和 RULE-SET）。使用 GitHub Actions 北京时间每天早上 6:30 自动构建，保证规则最新。

## 说明

本项目规则集（DOMAIN-SET 和 RULE-SET）的数据主要来源于项目 [@Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat) 和 [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community)；[`Apple`](https://github.com/Loyalsoldier/surge-rules/blob/release/apple.txt) 和 [`Google`](https://github.com/Loyalsoldier/surge-rules/blob/release/google.txt) 列表里的部分域名来源于项目 [@felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)；中国大陆 IPv4 地址数据使用 [@17mon/china_ip_list](https://github.com/17mon/china_ip_list)。

### ⚠️ 注意：

- **DOMAIN-SET** 同时适用于 Surge for Mac **v3.5.1** 及更新的版本、Surge for iOS **v4.2.2** 及更新的版本，拥有比 RULE-SET 更优秀的匹配效率，建议优先使用。
- **RULE-SET** 同时适用于 Surge for Mac **v3.0** 及更新的版本、Surge for iOS **v3.4** 及更新的版本。

## 规则文件地址及使用方式

### 在线地址（URL）

> 如果无法访问域名 `raw.githubusercontent.com`，可以使用第二个地址（`cdn.jsdelivr.net`），但是内容更新会有 12 小时的延迟。

#### DOMAIN-SET:

- **直连域名列表 direct.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/direct.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/direct.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/direct.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/direct.txt)
- **代理域名列表 proxy.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/proxy.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/proxy.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/proxy.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/proxy.txt)
- **广告域名列表 reject.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/reject.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/reject.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/reject.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/reject.txt)
- **私有网络专用域名列表 private.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/private.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/private.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/private.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/private.txt)
- **Apple 域名列表 apple.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/apple.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/apple.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/apple.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/apple.txt)
- **iCloud 域名列表 icloud.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/icloud.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/icloud.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/icloud.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/icloud.txt)
- **Google 域名列表 google.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/google.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/google.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/google.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/google.txt)
- **GFWList 域名列表 gfw.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/gfw.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/gfw.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/gfw.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/gfw.txt)
- **Greatfire 域名列表 greatfire.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/greatfire.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/greatfire.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/greatfire.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/greatfire.txt)
- **非中国大陆使用的顶级域名列表 tld-not-cn.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/tld-not-cn.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/tld-not-cn.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/tld-not-cn.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/tld-not-cn.txt)
- **Telegram 使用的 IP 地址列表 telegramcidr.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/telegramcidr.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/telegramcidr.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/telegramcidr.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/telegramcidr.txt)
- **中国大陆 IPv4 地址列表 cncidr.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/cncidr.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/cncidr.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/cncidr.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/cncidr.txt)

#### RULE-SET:

- **直连域名列表 direct.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/direct.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/direct.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/direct.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/direct.txt)
- **代理域名列表 proxy.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/proxy.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/proxy.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/proxy.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/proxy.txt)
- **广告域名列表 reject.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/reject.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/reject.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/reject.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/reject.txt)
- **私有网络专用域名列表 private.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/private.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/private.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/private.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/private.txt)
- **Apple 域名列表 apple.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/apple.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/apple.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/apple.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/apple.txt)
- **iCloud 域名列表 icloud.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/icloud.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/icloud.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/icloud.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/icloud.txt)
- **Google 域名列表 google.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/google.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/google.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/google.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/google.txt)
- **GFWList 域名列表 gfw.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/gfw.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/gfw.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/gfw.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/gfw.txt)
- **Greatfire 域名列表 greatfire.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/greatfire.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/greatfire.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/greatfire.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/greatfire.txt)
- **非中国大陆使用的顶级域名列表 tld-not-cn.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/tld-not-cn.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/tld-not-cn.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/tld-not-cn.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/tld-not-cn.txt)
- **Telegram 使用的 IP 地址列表 telegramcidr.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/telegramcidr.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/telegramcidr.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/telegramcidr.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/telegramcidr.txt)
- **中国大陆 IPv4 地址列表 cncidr.txt**：
  - [https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/cncidr.txt](https://raw.githubusercontent.com/Loyalsoldier/surge-rules/release/ruleset/cncidr.txt)
  - [https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/cncidr.txt](https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/cncidr.txt)

### 使用方式

关于 Surge 的详细使用方法，见[官方手册](https://manual.nssurge.com)。要想使用本项目的规则集，只需要在 Surge 配置文件中添加如下规则：

#### 白名单模式（推荐）

⚠️ 注意：

- 白名单模式，意为「**没有命中规则的网络流量，统统使用代理**」，适用于服务器线路网络质量稳定、快速，不缺服务器流量的用户。
- 以下配置中，除了 `DIRECT` 和 `REJECT` 是默认存在于 Surge 中的 policy（路由策略/流量处理策略），其余均为自定义 policy，对应配置文件中 `[Proxy]` 或 `[Proxy Group]` 中的代理名称。如你直接使用下面的 `[Rule]` 规则，则需要在 `[Proxy]` 或 `[Proxy Group]` 中手动配置一个名为 `PROXY` 的 policy。
- 如你希望 Apple、iCloud 和 Google 列表中的域名使用代理，则把 policy 由 `DIRECT` 改为 `PROXY`，以此类推，举一反三。

**DOMAIN-SET：**

```
[Rule]
PROCESS-NAME,v2ray,DIRECT
PROCESS-NAME,xray,DIRECT
PROCESS-NAME,clash,DIRECT
PROCESS-NAME,naive,DIRECT
PROCESS-NAME,trojan,DIRECT
PROCESS-NAME,trojan-go,DIRECT
PROCESS-NAME,ss-local,DIRECT
PROCESS-NAME,privoxy,DIRECT
PROCESS-NAME,leaf,DIRECT
PROCESS-NAME,Thunder,DIRECT
PROCESS-NAME,DownloadService,DIRECT
PROCESS-NAME,qBittorrent,DIRECT
PROCESS-NAME,Transmission,DIRECT
PROCESS-NAME,fdm,DIRECT
PROCESS-NAME,aria2c,DIRECT
PROCESS-NAME,Folx,DIRECT
PROCESS-NAME,NetTransport,DIRECT
PROCESS-NAME,uTorrent,DIRECT
PROCESS-NAME,WebTorrent,DIRECT
DOMAIN-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/private.txt,DIRECT
DOMAIN-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/reject.txt,REJECT
RULE-SET,SYSTEM,DIRECT
DOMAIN-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/icloud.txt,DIRECT
DOMAIN-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/apple.txt,DIRECT
DOMAIN-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/google.txt,DIRECT
DOMAIN-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/proxy.txt,PROXY,force-remote-dns
DOMAIN-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/direct.txt,DIRECT
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/telegramcidr.txt,PROXY
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/cncidr.txt,DIRECT
RULE-SET,LAN,DIRECT
FINAL,PROXY,dns-failed
```

**RULE-SET：**

```
[Rule]
PROCESS-NAME,v2ray,DIRECT
PROCESS-NAME,xray,DIRECT
PROCESS-NAME,clash,DIRECT
PROCESS-NAME,naive,DIRECT
PROCESS-NAME,trojan,DIRECT
PROCESS-NAME,trojan-go,DIRECT
PROCESS-NAME,ss-local,DIRECT
PROCESS-NAME,privoxy,DIRECT
PROCESS-NAME,leaf,DIRECT
PROCESS-NAME,Thunder,DIRECT
PROCESS-NAME,DownloadService,DIRECT
PROCESS-NAME,qBittorrent,DIRECT
PROCESS-NAME,Transmission,DIRECT
PROCESS-NAME,fdm,DIRECT
PROCESS-NAME,aria2c,DIRECT
PROCESS-NAME,Folx,DIRECT
PROCESS-NAME,NetTransport,DIRECT
PROCESS-NAME,uTorrent,DIRECT
PROCESS-NAME,WebTorrent,DIRECT
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/private.txt,DIRECT
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/reject.txt,REJECT
RULE-SET,SYSTEM,DIRECT
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/icloud.txt,DIRECT
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/apple.txt,DIRECT
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/google.txt,DIRECT
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/proxy.txt,PROXY,force-remote-dns
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/direct.txt,DIRECT
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/telegramcidr.txt,PROXY
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/cncidr.txt,DIRECT
RULE-SET,LAN,DIRECT
FINAL,PROXY,dns-failed
```

#### 黑色名单模式

⚠️ 注意：

- 黑名单模式，意为「**只有命中规则的网络流量，才使用代理**」，适用于服务器线路网络质量不稳定或不够快，或服务器流量紧缺的用户。通常也是软路由用户、家庭网关用户的常用模式。
- 以下配置中，除了 `DIRECT` 和 `REJECT` 是默认存在于 Surge 中的 policy（路由策略/流量处理策略），其余均为自定义 policy，对应配置文件中 `[Proxy]` 或 `[Proxy Group]` 中的代理名称。如你直接使用下面的 `[Rule]` 规则，则需要在 `[Proxy]` 或 `[Proxy Group]` 中手动配置一个名为 `PROXY` 的 policy。

**DOMAIN-SET：**

```
[Rule]
PROCESS-NAME,v2ray,DIRECT
PROCESS-NAME,clash,DIRECT
PROCESS-NAME,ss-local,DIRECT
PROCESS-NAME,privoxy,DIRECT
PROCESS-NAME,trojan,DIRECT
PROCESS-NAME,trojan-go,DIRECT
PROCESS-NAME,naive,DIRECT
PROCESS-NAME,Thunder,DIRECT
PROCESS-NAME,DownloadService,DIRECT
PROCESS-NAME,qBittorrent,DIRECT
PROCESS-NAME,Transmission,DIRECT
PROCESS-NAME,fdm,DIRECT
PROCESS-NAME,aria2c,DIRECT
PROCESS-NAME,Folx,DIRECT
PROCESS-NAME,NetTransport,DIRECT
PROCESS-NAME,uTorrent,DIRECT
PROCESS-NAME,WebTorrent,DIRECT
DOMAIN-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/private.txt,DIRECT
DOMAIN-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/reject.txt,REJECT
RULE-SET,SYSTEM,DIRECT
DOMAIN-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/tld-not-cn.txt,PROXY,force-remote-dns
DOMAIN-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/gfw.txt,PROXY,force-remote-dns
DOMAIN-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/greatfire.txt,PROXY,force-remote-dns
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/telegramcidr.txt,PROXY
FINAL,DIRECT,dns-failed
```

**RULE-SET：**

```
[Rule]
PROCESS-NAME,v2ray,DIRECT
PROCESS-NAME,clash,DIRECT
PROCESS-NAME,ss-local,DIRECT
PROCESS-NAME,privoxy,DIRECT
PROCESS-NAME,trojan,DIRECT
PROCESS-NAME,trojan-go,DIRECT
PROCESS-NAME,naive,DIRECT
PROCESS-NAME,Thunder,DIRECT
PROCESS-NAME,DownloadService,DIRECT
PROCESS-NAME,qBittorrent,DIRECT
PROCESS-NAME,Transmission,DIRECT
PROCESS-NAME,fdm,DIRECT
PROCESS-NAME,aria2c,DIRECT
PROCESS-NAME,Folx,DIRECT
PROCESS-NAME,NetTransport,DIRECT
PROCESS-NAME,uTorrent,DIRECT
PROCESS-NAME,WebTorrent,DIRECT
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/private.txt,DIRECT
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/reject.txt,REJECT
RULE-SET,SYSTEM,DIRECT
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/tld-not-cn.txt,PROXY,force-remote-dns
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/gfw.txt,PROXY,force-remote-dns
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/greatfire.txt,PROXY,force-remote-dns
RULE-SET,https://cdn.jsdelivr.net/gh/Loyalsoldier/surge-rules@release/ruleset/telegramcidr.txt,PROXY
FINAL,DIRECT,dns-failed
```

## 致谢

- [@Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)
- [@Loyalsoldier/cn-blocked-domain](https://github.com/Loyalsoldier/cn-blocked-domain)
- [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community)
- [@felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)
- [@17mon/china_ip_list](https://github.com/17mon/china_ip_list)
