---
description: 总结：审计大于加密，加密为审计服务
---

# 电商行业实施

### 电商行业背景描述（以深圳电商10-200人公司为例）：

需求提出人基本为公司老板or股东，很少有专门的IT从事人员负责运维。\
需求提出人一般更重视审计，唯一目的是审计员工是否有做什么其他事情，因此屏幕记录和IM记录至关重要。\
审计中，更重视的是微信的审计，但是现在做不到，因此引导客户去看屏幕记录为主。



### 服务器硬件参数需求评估标准

<table data-view="cards"><thead><tr><th>硬件描述</th><th></th><th data-hidden data-card-cover data-type="image">Cover image</th></tr></thead><tbody><tr><td>CPU</td><td>300人以下 8核</td><td><a href="https://images.unsplash.com/photo-1625315714730-d0830cd368bd?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxDUFV8ZW58MHx8fHwxNzYyNzQyMDEzfDA&#x26;ixlib=rb-4.1.0&#x26;q=85">https://images.unsplash.com/photo-1625315714730-d0830cd368bd?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxDUFV8ZW58MHx8fHwxNzYyNzQyMDEzfDA&#x26;ixlib=rb-4.1.0&#x26;q=85</a></td></tr><tr><td>内存</td><td>300人以下 16GB</td><td><a href="https://images.unsplash.com/photo-1541029071515-84cc54f84dc5?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxSQU18ZW58MHx8fHwxNzYyNzQyMDI0fDA&#x26;ixlib=rb-4.1.0&#x26;q=85">https://images.unsplash.com/photo-1541029071515-84cc54f84dc5?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxSQU18ZW58MHx8fHwxNzYyNzQyMDI0fDA&#x26;ixlib=rb-4.1.0&#x26;q=85</a></td></tr><tr><td>硬盘</td><td>按每100人一个月 1TB计算</td><td><a href="https://images.unsplash.com/photo-1597852074816-d933c7d2b988?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxIQVJEJTIwRFJJVkV8ZW58MHx8fHwxNzYyNzQyMDM2fDA&#x26;ixlib=rb-4.1.0&#x26;q=85">https://images.unsplash.com/photo-1597852074816-d933c7d2b988?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxIQVJEJTIwRFJJVkV8ZW58MHx8fHwxNzYyNzQyMDM2fDA&#x26;ixlib=rb-4.1.0&#x26;q=85</a></td></tr></tbody></table>

### 实施计划模板

{% stepper %}
{% step %}
### 安装服务器

服务器版本选择：能使用Windows Server 2019 / 2022 datacenter最好（因需要脚本部署）\
下载链接：[https://go.microsoft.com/fwlink/p/?LinkID=2195167\&clcid=0x804\&culture=zh-cn\&country=CN](https://go.microsoft.com/fwlink/p/?LinkID=2195167\&clcid=0x804\&culture=zh-cn\&country=CN)

\
数据库版本选择：使用 SQL Server 2019 /2022 版本，可使用免费的Express版本\
下载链接：[https://download.microsoft.com/download/7/f/8/7f8a9c43-8c8a-4f7c-9f92-83c18d96b681/SQL2019-SSEI-Expr.exe](https://download.microsoft.com/download/7/f/8/7f8a9c43-8c8a-4f7c-9f92-83c18d96b681/SQL2019-SSEI-Expr.exe)\
数据库下载后需手动选择下载安装介质：\
![](../../.gitbook/assets/image.png)\
![](<../../.gitbook/assets/image (1).png>)


{% endstep %}

{% step %}
### 确认部署逻辑


{% endstep %}

{% step %}
### 执行部署动作


{% endstep %}

{% step %}
### 后台整理名单


{% endstep %}

{% step %}
### 检查审计日志


{% endstep %}

{% step %}
### 数据分析分类


{% endstep %}

{% step %}
### 数据汇总报告


{% endstep %}
{% endstepper %}

