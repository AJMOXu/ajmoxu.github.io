---
title: 网页浏览
parent: IP-Guard
nav_order: 4
---

# 网页浏览

在开始之前，推荐先导入预定义的网址库 [网址库20221227.txt](https://github.com/AJMOXu/ajmoxu.github.io/files/10704304/20221227.txt)

## 网页浏览策略设置

此模块可以控制客户端的http(s)协议流量访问哪些域名

<mark style="color:red;">**因此需要注意的是**</mark>：如果使用白名单网页访问的情况下，可能存在部分应用的http(s)流量不正常的现象。

例如：微信发送图片、邮箱客户端登陆页面、部分应用二维码登录页面、部分应用内嵌页面等

### 以下是黑名单网页策略示例：

*   禁止管辖范围内的所有客户端访问财务与购物网站\
    &#x20;

    <figure><img src="https://user-images.githubusercontent.com/123937106/218020140-eaf91812-03cd-4fa2-a1a6-2c53d3f53cdb.png" alt=""><figcaption></figcaption></figure>

## 上传限制策略设置

此策略可以控制客户端的http(s)、TCP、ftp流量的上传文件大小限制

在高级->上传控制 中找到此策略设置 以下是策略示例：

* 禁止管辖范围内的所有客户端通过浏览器的http协议上传任何大于10KB的文件
* 同时禁止通过浏览器的ftp协议上传任何大于10KB的stp与dwg文件（不要纠结浏览器用ftp协议，演示用的，你也可以换成filezilla）
*   禁止通过浏览器的tcp协议往百度与阿里云上传任何大于10KB的文件（不要纠结浏览器用tcp协议，你也可以换成百度网盘，当然有些网盘应用不是用域名去连接服务器的，而是用IP）&#x20;

    <figure><img src="https://user-images.githubusercontent.com/123937106/218021050-01b8cfcf-95f4-4be3-8e25-999a09b79d68.png" alt=""><figcaption></figcaption></figure>

## 网页浏览日志查询

在日志->网页浏览 中找到网页浏览日志

记录了客户端上访问网页时的网址和网站域名，以及标题（浏览器打开本地PDF时，标题会显示为文件名，网址会显示为file//开头）\
&#x20;

<figure><img src="https://user-images.githubusercontent.com/123937106/218030365-cdf31ad8-e7af-469c-8711-aad8d596fccb.png" alt=""><figcaption></figcaption></figure>

## 网页浏览联动功能

### 联动文档水印功能示例：

*   管辖范围内所有客户端将office、pdf、图像文件通过网络传输到带有”pan“”aliyun“”git“关键字的网址时，会自动添加水印 \


    <figure><img src="https://user-images.githubusercontent.com/123937106/218032245-52d665a9-7182-48a3-8580-7880bab4c6d9.png" alt=""><figcaption></figcaption></figure>

### 联动屏幕监控功能示例：

*   管辖范围内所有客户端访问到求职网站、网盘网站时，自动在其页面访问到时对屏幕进行触发式屏幕记录（默认2s一次，一共三次） \


    <figure><img src="https://user-images.githubusercontent.com/123937106/218032811-fc6a7e02-e24c-44f1-8a15-4349c53c727e.png" alt=""><figcaption></figcaption></figure>
