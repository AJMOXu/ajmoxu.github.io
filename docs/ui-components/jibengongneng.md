---
layout: default
title: 基本功能
parent: IP-Guard
nav_order: 2
---

基本策略示例
{: .fs-6 }
假如您的需求是：在公司时禁止修改 IP 地址，但是允许回家或出差的时候修改IP。管理员可以对目标计算机（如整个网络）设置基本策略：


- 先设置一条策略，禁止修改 IP/MAC 属性

<img width="1280" alt="simple" src="https://user-images.githubusercontent.com/123937106/215726448-e1dee8d0-4b86-4398-9693-484cb348266c.png">


- 再设置一条离线策略，允许 修改 IP/MAC 属性 仅离线生效

<img width="1280" alt="simple2" src="https://user-images.githubusercontent.com/123937106/215726504-469a1951-0372-4700-9d90-5c0ed8852832.png">


按照策略匹配原则，后设置的策略在上面，因此策略2优先于策略1，当离线状态时，策略匹配，允许修改 IP/MAC；当在线状态时，与策略2不匹配，接着向下匹配策略1，条件满足，执行策略禁止修改 IP/MAC 属性。
{: 	.text-red-300 }

基本日志查询
{: .fs-6 }

选择菜单“日志->基本事件”查看基本事件日志，基本事件日志记录客户端系统的启动/停止，用户登录/注销，拨号，补丁管理和软件分发相关日志。
<img width="1142" alt="rizhi" src="https://user-images.githubusercontent.com/123937106/215730143-8a880907-7624-44a2-b075-6c83fbc2b538.png">



服务器各功能设置
{: .fs-6 }

