---
layout: default
title: 应用程序
parent: IP-Guard
nav_order: 3
---

应用程序策略设置
{: .fs-6 }

在选项卡：策略->应用程序 中找到此策略设置界面
以下为策略设置示例：
- 禁止所有管辖范围内客户端使用软件QQ或运行名称为 "qq.exe" 的应用程序
<img width="1280" alt="yingyongchengxu" src="https://user-images.githubusercontent.com/123937106/215986529-3e42fd85-d1ff-4d96-8c15-04afd81da225.png">


软件安装策略设置
{: .fs-6 }

在选项卡：策略->软件安装管理 中找到此策略设置界面
以下为策略设置示例：
- 禁止所有管辖范围内客户端安装任何应用程序，仅允许安装360
- 同时禁止所有管辖范围内客户端卸载任何应用
<img width="1280" alt="软件安装管理" src="https://user-images.githubusercontent.com/123937106/218008460-3f60bc80-e82d-4557-a629-4c7648856e01.png">

- 软件安装包分类库需要管理员自行上传维护
- 以下是软件安装包分类库添加示例
在分类管理->软件安装包 中找到软件安装包分类库
<img width="1280" alt="微信截图_20230210133129" src="https://user-images.githubusercontent.com/123937106/218009185-e9663926-2d22-4b4e-b222-922da0eb4be6.png">

如图所示添加软件安装包即可
<img width="1280" alt="软件安装包分类库" src="https://user-images.githubusercontent.com/123937106/218009831-20e4975a-3fe8-46cf-9f61-8c1462b00aba.png">



应用程序日志查询
{: .fs-6 }

在选项卡：日志->应用程序 中找到此模块日志面板
记录客户端上所有应用程序的启停行为，以及应用程序路径，支持筛选
<img width="1280" alt="yingyongchengxu2" src="https://user-images.githubusercontent.com/123937106/215987059-df0ba60b-8392-431f-9230-071d8ac29dec.png">



应用程序联动功能
{: .fs-6 }

在菜单栏：分类管理->应用程序 中，可以查询到应用程序库
<img width="1280" alt="yingyongchengxu3" src="https://user-images.githubusercontent.com/123937106/215987368-9efa2ea6-1153-40f1-9ab3-fd26210fc2f0.png">

在默认情况下，IPG会将所有记录到的应用程序信息保存在 应用程序库->未分类 类别中
以下为示例：
- 在应用程序库中查找未分类的应用程序
- 筛选应用名称包含 “qq” 字样的应用程序
- 选中一部分筛选出的应用程序，将其识别规则放入分类 “QQ” 中
- 在网络控制模块中，调用 “QQ” 类别应用程序，禁止此类别中的应用程序联网
<img width="1280" alt="yingyongchengxu4" src="https://user-images.githubusercontent.com/123937106/215988354-5dea041a-cc57-47d3-8704-69cc629ef0f0.png">
<img width="1280" alt="yingyongchengxu5" src="https://user-images.githubusercontent.com/123937106/215988503-03f76a14-7b1e-496e-969a-3253a0b28970.png">



