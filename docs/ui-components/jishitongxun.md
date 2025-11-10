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


    <figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

***



### 允许客户端使用所有IM工具发送文件和图片，并备份外传的所有文件和图片，同时记录外发时的屏幕

* 在【高级】→【IM文件传送】中，新建策略，【动作】选择【允许】，勾选【文件控制】【图片控制】及【是否备份】，在最底端的【聊天工具】中选择全部的IM工具

#### IM工具 发送文件 和 接收文件 备份策略示例

*   备份所有IM工具发送的文件和图片，并记录外发时的屏幕\


    <figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>


*   备份所有IM工具接收的文件和图片\


    <figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
备份接收的文件和图片流量可能会很大

即使是群聊的消息和图片也会自动备份

接收文件备份不支持触发屏幕记录
{% endhint %}



***



## 即时通讯日志查询

### 查询用户通过什么IM工具发送了哪些内容

*   在【监视】→【即时通讯】中，默认会展示最近30天的聊天记录，如需查找指定时间段或更长时间的，在右侧筛选框中选择对应的功能\


    <figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>
*   如需查找特定的文字内容或者文件，在右边筛选框的【内容】项中，输入关键字即可，默认模糊匹配，支持文件名

    <figure><img src="../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

***



## 微信当前不再支持默认的记录方式

### 当前支持的微信记录方式

* 利用【屏幕记录】，记录【wechat.exe】运行时的所有屏幕内容
* 利用【上传备份】，记录【wechat.exe】上传的所有文件

#### 屏幕记录策略示例

<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

#### 上传备份策略示例

<figure><img src="../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

***
