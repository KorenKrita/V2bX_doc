---
description: A Xray backend framework that can easily support many panels.
---

# 关于V2bX

## V2bX

A V2board node server based on Xray-core, modified from XrayR

一个基于Xray-core的V2board节点服务端，修改自XrayR，支持V2ay,Trojan,Shadowsocks,Hysteria协议。

本项目为基于原始[V2bX](https://github.com/InazumaV/V2bX)[V2board](https://github.com/wyx2685/v2board)。

## 项目目录

* [V2bX](https://github.com/wyx2685/V2bX)：V2bX源码以及软件发布。
* [V2bX-script](https://github.com/wyx2685/V2bX-script)：V2bX一键安装脚本。
* [V2bX\_doc](https://github.com/wyx2685/V2bX\_doc)：V2bX文档源码。

## 特点

* 永久开源且免费。
* 支持V2ray，Trojan， Shadowsocks，Hysteria多种协议。
* 支持Vless和XTLS等新特性。
* 支持单实例对接多面板、多节点，无需重复启动。
* 支持跨节点限制在线IP
* 支持节点级别、用户级别限速。
* 配置简单明了。
* 修改配置自动重启实例。
* 方便编译和升级，可以快速更新核心版本， 支持Xray-core，Sing-box，Hysteria新特性。

## 功能介绍

| 功能        | v2ray | trojan | shadowsocks | Hysteria |
| --------- | ----- | ------ | ----------- | -------- |
| 获取节点信息    | √     | √      | √           | √        |
| 获取用户信息    | √     | √      | √           | √        |
| 用户流量统计    | √     | √      | √           | √        |
| 服务器信息上报   | √     | √      | √           | √        |
| 自动申请tls证书 | √     | √      | √           | √        |
| 自动续签tls证书 | √     | √      | √           | √        |
| 在线人数统计    | √     | √      | √           | √        |
| 在线用户限制    | √     | √      | √           | √        |
| 审计规则      | √     | √      | √           | √        |
| 节点端口限速    | √     | √      | √           | √        |
| 按照用户限速    | √     | √      | √           | √        |
| 自定义DNS    | √     | √      | √           | √        |

## V2ray支持协议

| 协议        | 支持情况                                                                                |
| --------- | ----------------------------------------------------------------------------------- |
| VMess     | tcp, tcp+http, tcp+tls, ws, ws+tls, h2c, h2+tls, grpc, grpc+tls                     |
| VMessAEAD | tcp, tcp+http, tcp+tls, ws, ws+tls, h2c, h2+tls, grpc, grpc+tls                     |
| VLess     | tcp, tcp+http, tcp+tls/xtls, ws, ws+tls/xtls, h2c, h2+tls/xtls, grpc, grpc+tls/xtls |

## Trojan支持协议

| 协议     | 支持情况 |
| ------ | ---- |
| Trojan | √    |

## Shadowsocks支持协议

| 协议              | 支持情况 | 加密方法                                             |
| --------------- | ---- | ------------------------------------------------ |
| ShadowsocksAEAD | √    | aes-128-gcm, aes-256-gcm, chacha20-ietf-poly1305 |

## Hysteria支持协议

<table><thead><tr><th>协议</th><th>支持情况</th><th data-hidden>加密方法</th><th data-hidden></th></tr></thead><tbody><tr><td>Hysteria</td><td>√</td><td></td><td></td></tr><tr><td>Hysteria2</td><td>√</td><td>aes-128-gcm, aes-256-gcm, chacha20-ietf-poly1305</td><td></td></tr></tbody></table>
