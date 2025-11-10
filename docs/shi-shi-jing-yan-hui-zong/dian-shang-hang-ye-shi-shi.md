---
description: 总结：审计大于加密，加密为审计服务
---

# 电商行业实施

## 电商行业背景描述（以深圳电商10-200人公司为例）：

需求提出人基本为公司老板or股东，很少有专门的IT从事人员负责运维。\
需求提出人一般更重视审计，唯一目的是审计员工是否有做什么其他事情，因此屏幕记录和IM记录至关重要。\
审计中，更重视的是微信的审计，但是现在做不到，因此引导客户去看屏幕记录为主。



## 服务器硬件参数需求评估标准

{% hint style="info" %}
<p align="center"><strong>主服务器</strong></p>
{% endhint %}

<table data-view="cards"><thead><tr><th>硬件描述</th><th></th><th data-hidden data-card-cover data-type="image">Cover image</th></tr></thead><tbody><tr><td>CPU</td><td>300人以下 8核</td><td><a href="https://images.unsplash.com/photo-1625315714730-d0830cd368bd?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxDUFV8ZW58MHx8fHwxNzYyNzQyMDEzfDA&#x26;ixlib=rb-4.1.0&#x26;q=85">https://images.unsplash.com/photo-1625315714730-d0830cd368bd?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxDUFV8ZW58MHx8fHwxNzYyNzQyMDEzfDA&#x26;ixlib=rb-4.1.0&#x26;q=85</a></td></tr><tr><td>内存</td><td>300人以下 16GB</td><td><a href="https://images.unsplash.com/photo-1541029071515-84cc54f84dc5?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxSQU18ZW58MHx8fHwxNzYyNzQyMDI0fDA&#x26;ixlib=rb-4.1.0&#x26;q=85">https://images.unsplash.com/photo-1541029071515-84cc54f84dc5?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxSQU18ZW58MHx8fHwxNzYyNzQyMDI0fDA&#x26;ixlib=rb-4.1.0&#x26;q=85</a></td></tr><tr><td>硬盘</td><td>按每100人一个月 1TB计算</td><td><a href="https://images.unsplash.com/photo-1597852074816-d933c7d2b988?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxIQVJEJTIwRFJJVkV8ZW58MHx8fHwxNzYyNzQyMDM2fDA&#x26;ixlib=rb-4.1.0&#x26;q=85">https://images.unsplash.com/photo-1597852074816-d933c7d2b988?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxIQVJEJTIwRFJJVkV8ZW58MHx8fHwxNzYyNzQyMDM2fDA&#x26;ixlib=rb-4.1.0&#x26;q=85</a></td></tr></tbody></table>

{% hint style="info" %}
<p align="center">数据分析预警服务器</p>
{% endhint %}

<table data-view="cards"><thead><tr><th></th><th></th><th data-hidden data-card-cover data-type="image">Cover image</th></tr></thead><tbody><tr><td>CPU</td><td>500人以下16核</td><td><a href="https://images.unsplash.com/photo-1625315714730-d0830cd368bd?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxDUFV8ZW58MHx8fHwxNzYyNzQyMDEzfDA&#x26;ixlib=rb-4.1.0&#x26;q=85">https://images.unsplash.com/photo-1625315714730-d0830cd368bd?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxDUFV8ZW58MHx8fHwxNzYyNzQyMDEzfDA&#x26;ixlib=rb-4.1.0&#x26;q=85</a></td></tr><tr><td>内存</td><td>500人以下32GB</td><td><a href="https://images.unsplash.com/photo-1541029071515-84cc54f84dc5?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxSQU18ZW58MHx8fHwxNzYyNzQyMDI0fDA&#x26;ixlib=rb-4.1.0&#x26;q=85">https://images.unsplash.com/photo-1541029071515-84cc54f84dc5?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxSQU18ZW58MHx8fHwxNzYyNzQyMDI0fDA&#x26;ixlib=rb-4.1.0&#x26;q=85</a></td></tr><tr><td>硬盘</td><td>1TB</td><td><a href="https://images.unsplash.com/photo-1597852074816-d933c7d2b988?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw2fHxIRER8ZW58MHx8fHwxNzYyNzQ2OTUwfDA&#x26;ixlib=rb-4.1.0&#x26;q=85">https://images.unsplash.com/photo-1597852074816-d933c7d2b988?crop=entropy&#x26;cs=srgb&#x26;fm=jpg&#x26;ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw2fHxIRER8ZW58MHx8fHwxNzYyNzQ2OTUwfDA&#x26;ixlib=rb-4.1.0&#x26;q=85</a></td></tr></tbody></table>



## 实施步骤及计划说明



{% stepper %}
{% step %}
### 安装服务器

{% tabs %}
{% tab title="主服务器" %}
服务器版本选择：能使用Windows Server 2019 / 2022 datacenter最好（因需要脚本部署）\
下载链接：[https://go.microsoft.com/fwlink/p/?LinkID=2195167\&clcid=0x804\&culture=zh-cn\&country=CN](https://go.microsoft.com/fwlink/p/?LinkID=2195167\&clcid=0x804\&culture=zh-cn\&country=CN)\
服务器配置要求：[https://learn.microsoft.com/zh-cn/windows-server/get-started/hardware-requirements?tabs=cpu\&pivots=windows-server-2019](https://learn.microsoft.com/zh-cn/windows-server/get-started/hardware-requirements?tabs=cpu\&pivots=windows-server-2019)

\
数据库版本选择：使用 SQL Server 2019 /2022 版本，可使用免费的Express版本\
下载链接：[https://download.microsoft.com/download/7/f/8/7f8a9c43-8c8a-4f7c-9f92-83c18d96b681/SQL2019-SSEI-Expr.exe](https://download.microsoft.com/download/7/f/8/7f8a9c43-8c8a-4f7c-9f92-83c18d96b681/SQL2019-SSEI-Expr.exe)\
数据库下载后需手动选择下载安装介质：\
![](../../.gitbook/assets/image.png)\
![](<../../.gitbook/assets/image (1).png>)



安装注意事项：

* 推荐使用运行盘+数据盘的部署方式，即操作系统和主服务器安装在运行盘，数据定期转移到数据盘
* 安装时应注意设置混合登陆模式并设置sa账户密码
{% endtab %}

{% tab title="Web服务器" %}
版本无特殊要求，跟随主服务器版本安装正确的版本即可

Web服务器主要作为分发给人事/行政同事的管理平台使用，具备轻量化，易操作的优点，对于文职岗位的管理人员来说，更容易上手

Web服务器部署时，应选择自生成Https的SSL证书，并为Https协议设置端口号，一般建议为标准端口号443加上前缀，例如 30443

Web服务器部署后，应更换Web服务器的产品LOGO为公司LOGO。

LOGO参数要求：\
导航栏LOGO，像素大小为130\*31，格式为svg格式，应命名为logo.svg\
标签页LOGO，像素大小为16\*16，格式为ico格式，应命名为console.ico

LOGO替换脚本：

{% code title="创建双击替换web控制台logo.bat文件，使用记事本打开bat文件编写以下脚本" fullWidth="true" %}
```batch
set LogoPath=C:\Program Files (x86)\TEC\WebServer\

cd ~dp0
copy logo.svg "%LogoPath%www\ipg\static\img\logo.svg" /y
copy logo.svg "%LogoPath%www\ipg\static\console\img\logo.svg" /y
copy logo.svg "%LogoPath%www\ipg\static\appr\images\logo.svg" /y
copy logo.svg "%LogoPath%www\ipg\static\report\images\logo.svg" /y
copy logo.svg "%LogoPath%www\ipg\static\img\logo.svg" /y
copy console.ico "%LogoPath%www\favicon.ico" /y
copy console.ico "%LogoPath%www\ipg\static\img\favicon.ico" /y
copy console.ico "%LogoPath%www\ipg\static\console\img\console.ico" /y

exit;
```
{% endcode %}

111\.

1
{% endtab %}

{% tab title="数据分析预警服务器" %}
服务器版本：推荐使用Ubuntu 20以上的操作系统版本，使用rufus封装镜像到U盘安装操作系统\
镜像下载链接(Ubuntu 24.04)：[https://ubuntu.com/download/desktop/thank-you?version=24.04.3\&architecture=amd64\&lts=true](https://ubuntu.com/download/desktop/thank-you?version=24.04.3\&architecture=amd64\&lts=true)

按照文档安装即可，其他无要求，缺少相关软件时注意更换为国内下载源

1安装完之后需要配置数据同步范围，默认只有30天的同步范围，如果想扩展，则需要进行以下更改

1. 设置服务器保留日志数据库时间范围

{% code overflow="wrap" %}
```batch
--设置配置
USE [OCULAR3]
DECLARE @SC_INT int
DECLARE @SC_STR NVARCHAR(255)
SET @SC_INT = 2
SET @SC_STR = N'
<DATA>
    <DAYS>30</DAYS>
</DATA>'
IF EXISTS (SELECT * FROM SYS_CFG WHERE SC_NAME =N'DataLoadMode')
    UPDATE SYS_CFG SET SC_INT = @SC_INT, SC_STR = @SC_STR WHERE SC_NAME = N'DataLoadMode'
ELSE
    INSERT INTO SYS_CFG(SC_NAME, SC_INT, SC_STR) VALUES(N'DataLoadMode', @SC_INT, @SC_STR)
--查看配置
SELECT * FROM SYS_CFG WHERE SC_NAME = N'DataLoadMode'
SC_INT设置加载模式，
SC_INT为0时表示不加载，
SC_INT为1时表示加载所有的，
SC_INT为2时表示加载最近多少天内的日志数据库，加载的天数从SC_STR读取，SC_STR是一个XML结构，如上述SQL语句中所写。
SC_INT为3时表示加载某段日期内的日志数据库，加载的日期范围从SC_STR读取，SC_STR是一个XML结构，形如：

<DATA>
    <FROM>20130201</FROM>
    <TO>20130310</TO>
</DATA>
```
{% endcode %}

2. 批量附加数据库

{% code overflow="wrap" %}
```batch
SET NOCOUNT ON
USE [OCULAR3]
GO

IF EXISTS (SELECT * FROM SYSOBJECTS WHERE [name] = 'p_BatchAttachDB' AND [xtype] = 'P')
	DROP PROCEDURE [p_BatchAttachDB]
GO

CREATE PROCEDURE [p_BatchAttachDB] @dateBegin DATETIME, @dateEnd DATETIME, @dir NVARCHAR(255)
AS
BEGIN
	IF RIGHT(@dir, 1) <> '\'
		SET @dir = @dir + '\'
	PRINT N'当前数据目录：' + @dir
	PRINT N'-----------------------'

	DECLARE @DATE DATETIME
	DECLARE @CURDATE INT
	DECLARE @CURINDEX INT
	DECLARE @DBNAME NVARCHAR(255)
	DECLARE @FILENAME NVARCHAR(255)
	DECLARE @ISEXISTS INT
	SET @DATE=@dateBegin
	WHILE (@DATE<=@dateEnd)
	BEGIN
		SET @CURDATE=YEAR(@DATE)*10000+MONTH(@DATE)*100+DAY(@DATE)
		SET @CURINDEX = -1
		WHILE @CURINDEX < 8
		BEGIN
			IF @CURINDEX = -1
				SET @DBNAME='OCULAR3_DATA.'+CAST(@CURDATE AS NVARCHAR(8))
			ELSE
				SET @DBNAME='OCULAR3_DATA.'+CAST(@CURDATE AS NVARCHAR(8)) + '.' + CAST(@CURINDEX AS NVARCHAR(1))

			SET @FILENAME=@dir+@DBNAME+'.MDF'
			EXEC master.dbo.xp_fileexist @FILENAME, @ISEXISTS OUTPUT
			IF @ISEXISTS = 1
			BEGIN
				IF NOT EXISTS(SELECT * FROM MASTER.DBO.SYSDATABASES WHERE NAME = @DBNAME)
					EXEC SP_ATTACH_DB @DBNAME, @FILENAME
				PRINT @DBNAME + '已附加'
			END
			SET @CURINDEX = @CURINDEX + 1
		END
		SET @DATE=@DATE+1
	END
END
GO

--自定义
DECLARE @B_DATE DATETIME
DECLARE @E_DATE DATETIME
DECLARE @DIR NVARCHAR(255)
SET @B_DATE = '2013-06-01'			-- 起始日期
SET @E_DATE = '2013-06-23'			-- 结束日期
SET @DIR = N'E:\OServer3\DATA\'		-- DATA目录
EXEC [p_BatchAttachDB] @B_DATE, @E_DATE, @DIR
GO

IF EXISTS (SELECT * FROM SYSOBJECTS WHERE [name] = 'p_BatchDetachDB' AND [xtype] = 'P')
	DROP PROCEDURE [p_BatchDetachDB]
GO
```
{% endcode %}

4
{% endtab %}
{% endtabs %}












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

