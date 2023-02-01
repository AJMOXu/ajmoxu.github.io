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

设置管理员账号
{: .fs-5 }

<img width="1280" alt="zhanghao" src="https://user-images.githubusercontent.com/123937106/215958079-56274cbb-fc70-46d5-9fba-a43ea91b0820.png">

<img width="1280" alt="zhanghao2" src="https://user-images.githubusercontent.com/123937106/215958386-42af8f4d-6304-4203-8844-5f8854642289.png">

<img width="1280" alt="zhuoguan3" src="https://user-images.githubusercontent.com/123937106/215958685-2c232369-ff71-453a-9a4c-0e9fe9509b60.png">

根据账号设置审批流程
{: .fs-5 }

<img width="1280" alt="zhuoguanshenpi" src="https://user-images.githubusercontent.com/123937106/215958997-8e6b5ee4-eb87-4a1a-91b8-80e363f92e53.png">

在此处设置桌管审批范围与内容
<img width="1280" alt="zhuoguanshenpi2" src="https://user-images.githubusercontent.com/123937106/215959149-6ba29f3f-4e40-4210-8196-b909fdfc8b1a.png">

在此处设置桌管审批流程与对象
<img width="1280" alt="zhuoguanshenpi3" src="https://user-images.githubusercontent.com/123937106/215959307-fbf89e3b-80b1-407c-a879-a427503c39aa.png">

需要注意的是，审批流程是自上而下匹配的，如一个客户端的申请有多条审批流程可匹配时，只匹配自上而下第一个符合设置的流程
{: 	.text-red-300 }


设置备份数据
{: .fs-5 }

<img width="1280" alt="shujubeifen" src="https://user-images.githubusercontent.com/123937106/215960035-2e3a0c64-0557-417f-b248-6770c496d201.png">

在此处可设置需要备份的内容与范围
<img width="1280" alt="shujubeifen2" src="https://user-images.githubusercontent.com/123937106/215960070-89ef8a29-7ff8-4319-96ce-d174d5a63f31.png">

以下是一个备份示例：
- 备份自2022\04\01以来所有的文档操作日志以及文档操作日志备份的文件副本
- 备份数据存储至 N:\ 盘 根目录下
- 同时删除原有的数据，腾出主服务器存储目录空间
<img width="1280" alt="shujubeifen3" src="https://user-images.githubusercontent.com/123937106/215960298-196cb0a7-a1e7-4a5c-8f67-876b69b27a37.png">


在此处可设置定期自动备份，以下是一个备份案例：
- 每月1日下午13:38分自动备份上一个月的所有数据信息
- 备份数据存储至 C:\ 盘 根目录下
- 同时删除原有的数据，腾出主服务器存储目录空间
<img width="1280" alt="shujubeifen4" src="https://user-images.githubusercontent.com/123937106/215960988-60503345-1696-436f-8d3d-25b635b9e1e9.png">

需要注意的是，如果您选择了备份数据至网络路径，需要设置此策略的PC和服务器均能访问到指定网络路径
{: 	.text-red-300 }

在此处可加载指定备份，加载的备份不会占用主服务器存储空间，就像打开指定位置的文件一样
<img width="1280" alt="shujubeifen5" src="https://user-images.githubusercontent.com/123937106/215961344-70e7ed65-bfb7-4e93-ba74-d7896d6feaa2.png">


组织架构同步（LDAP，AD域等）
{: .fs-5 }

<img width="1280" alt="jiagoutongbu" src="https://user-images.githubusercontent.com/123937106/215961632-b39ce36f-e001-4449-bd45-252686af50c1.png">

组织架构同步示例（AD域）：
- 同步AJMOXu.com的所有域组织架构到IPG根组织架构
- 自动根据AJMOXu.com域中用户的组织架构位置，将用户所登陆的客户端计算机同步到IPG组织架构
- 对于没有对象的OU不进行导入
- 自动将用户初次登录的计算机与用户关联
<img width="1280" alt="jiagoutongbu3" src="https://user-images.githubusercontent.com/123937106/215963016-b07b2806-a18d-4833-a7c5-f05f54d3b7e0.png">

需要注意的是，用户初次登陆的客户端与用户会自动关联，此关联信息影响到此客户端在IPG的计算机组织架构中的位置，并且关联信息不会自动清除，需要手动清除
{: 	.text-red-300 }


客户端离线卸载与离线策略消除
{: .fs-5 }

在此处找到客户端离线辅助工具
<img width="1280" alt="fuzhugongju" src="https://user-images.githubusercontent.com/123937106/215984895-cf62bc69-a0de-4c98-a158-8da86b8e0c72.png">

选择卸载客户端或临时清除策略（此处以卸载客户端为演示）
<img width="1280" alt="fuzhugongju2" src="https://user-images.githubusercontent.com/123937106/215985053-6ec3b016-9e61-4d5e-9b1f-1d7b85a449f2.png">

设置卸载工具各项参数，以下为演示：
- 工具可用10次
- 工具可用时间1天
- 工具密码为123
- 工具导出路径为  C:\Users\85471\Desktop\agttool.exe
<img width="1280" alt="fuzhugongju3" src="https://user-images.githubusercontent.com/123937106/215985369-bd9a3baf-43a9-4a34-8e24-a1f0ccafff60.png">

将此工具拿到客户端上执行，输入正确密码即可离线卸载客户端








