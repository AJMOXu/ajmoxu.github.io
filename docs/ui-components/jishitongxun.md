---
title: 即时通讯
parent: IP-Guard
nav_order: 10
icon: weixin
---

# 即时通讯

## 即时通讯策略设置

### 禁止客户端使用某一个IM工具发送文件或图片

* 在【高级】→【IM文件传送】中，新建策略，【动作】选择【禁止】，勾选【文件控制】【图片控制】，在最底端的【聊天工具】中选择需要禁止的IM工具

#### 策略示例

*   禁止除了【企业微信】外，所有IM工具发送文件\
    \


    <figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

***



### 允许客户端使用所有IM工具发送文件和图片，并备份外传的所有文件和图片，同时记录外发时的屏幕

* 在【高级】→【IM文件传送】中，新建策略，【动作】选择【允许】，勾选【文件控制】【图片控制】及【是否备份】，在最底端的【聊天工具】中选择全部的IM工具

#### IM工具 发送文件 和 接收文件 备份策略示例

*   备份所有IM工具发送的文件和图片，并记录外发时的屏幕\


    <figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>


*   备份所有IM工具接收的文件和图片\


    <figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
备份接收的文件和图片流量可能会很大

即使是群聊的消息和图片也会自动备份

接收文件备份不支持触发屏幕记录
{% endhint %}

## 即时通讯日志查询

## 即时通讯联动功能
