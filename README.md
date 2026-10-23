# Anywhere 直连规则订阅

供 Anywhere 应用使用的三个直连规则集。文件均为 UTF-8 格式，设置 `routing = 1`（DIRECT）。

## 订阅地址（Raw）

1. **直连域名 1**（100,000 条域名规则）  
   https://raw.githubusercontent.com/lovebaba1069/anywhere-direct-rules/main/rules/Direct-Domains-1.arrs

2. **直连域名 2**（12,201 条域名规则）  
   https://raw.githubusercontent.com/lovebaba1069/anywhere-direct-rules/main/rules/Direct-Domains-2.arrs

3. **直连 IP 网段**（6,545 条 IPv4 + 3,493 条 IPv6，共 10,038 条）  
   https://raw.githubusercontent.com/lovebaba1069/anywhere-direct-rules/main/rules/Direct-IP.arrs

## 格式

- 域名后缀：`2, example.com`
- IPv4 CIDR：`0, 1.2.3.0/24`
- IPv6 CIDR：`1, 2001:db8::/32`

导入 Anywhere 的网络规则订阅时，分别添加以上三个 Raw URL，并选择直连策略。请注意规则集顺序与优先级，避免意外覆盖已有的苹果服务、iCloud+ 等代理规则。

## 说明

文件存放在仓库的 `rules/` 子目录，旧的“不带 rules/”的根目录 URL 并不指向本次上传的文件。对三个 .arrs 文件的后续修改会反映到这些固定 Raw 地址。

## 订阅图标

三个 .arrs 文件均内嵌同一张自定义人像图标（192×192 JPEG，约 4.8 KB），以 `icon-light` 与 `icon-dark` 提供亮色及暗色主题支持。原有规则和 Raw URL 均保持不变。图标随公开规则文件一起公开。
