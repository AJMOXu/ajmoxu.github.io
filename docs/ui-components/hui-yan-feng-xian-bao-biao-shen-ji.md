---
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 📊 慧眼风险报表审计

报表UI说明

*   实用的几个功能都集中在上方导航栏的【报表】选项栏中\


    <figure><img src="../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

### 报表-模板管理

#### 新建报表模板

* 默认模板无法更改
*   根据不同的功能模块，有不同的模板设置，模板对应不同的模块\


    <figure><img src="../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>
*   右键手动创建模板\


    <figure><img src="../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>
*   模板条件设置和对应模块的日志筛选框一样\
    示例：筛选所有用户，所有计算机的微信上传文件日志，以计算机为基准统计出来\


    <figure><img src="../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

***





## 趋势表|统计表|征兆表的区别和用法

### 趋势表

#### 趋势表用途场景

*   用于发现某一个时间段是否有大批量的上传，例如：发现某一日某个用户的上传日志超出平均值很多\


    <figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>
* 用于评估内网的平均上传大小，获取到合适的数据用于【征兆表】的创建

#### 如何创建趋势表

*   右键报表分组，新建报表，选择【从查询条件创建】\


    <figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>
*   选择需要创建的趋势表，例如这里我想筛选文档操作相关的日志，就选【标准文档操作趋势表】\


    <figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>
*   筛选感兴趣的日志，例如截图中筛选的是所有删除用户手动删除的日志。然后点击【下一步】\


    <figure><img src="../../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>
*   选择统计单位（时间间隔，最短一天）和统计类型（统计用户的行为，还是计算机行为）然后【下一步】\


    <figure><img src="../../.gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>
*   选择报表统计的周期时间，这里选择【标准月】即可，然后【下一步】\


    <figure><img src="../../.gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>
*   命名报表名称，然后点击【完成】\


    <figure><img src="../../.gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>
*   创建后不会自动立即统计过往数据，需要到【报表】-【生成历史报表】-选择刚创建的报表-选择生成的时间范围，保存后才能开始统计过往数据（统计需要时间）\


    <figure><img src="../../.gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>

***



### 统计表

#### 统计表用途场景

*   用于直观的看到一段时间内的各项数据的总数据大小，例如图中展示的是2024年11月的删除、上传、下载文件数量和大小

    <figure><img src="../../.gitbook/assets/image (7) (1).png" alt=""><figcaption></figcaption></figure>
*   结合【资产管理模块】，统计内网软硬件资产\


    <figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

#### 创建统计表（与趋势表一样）

*   右键报表分组，新建报表，选择【从查询条件创建】

    <figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>
*   根据需要选择对应模块报表，这里依旧选择【文档操作报表】\


    <figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>
* 之后的操作和趋势表一样，这里就不再补充了，如果需要补充请联系我

***

### 征兆表

#### 征兆表用途场景

* 根据[趋势表中获取的数据平均值](hui-yan-feng-xian-bao-biao-shen-ji.md#qu-shi-biao-yong-tu-chang-jing)，来制定平均水平线，设定超过该平均线的行为是危险行为，并自动统计到日报，结合邮件报告隔日提醒
* 设定黑名单或白名单上传地址，用户一旦有黑名单或白名单之外的操作自动统计为危险行为，结合邮件报告隔日提醒

#### 如何创建征兆表

*   需要先制定征兆行为（既风险行为），选择【报表】-【征兆条件设置】\


    <figure><img src="../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>
*   选择【增加】，根据日志数据类型创建征兆条件，这里依旧选择文档操作日志为基准

    <figure><img src="../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>
*   设定【1分钟内】删除文件超过50个或删除文件大小大于5GB为严重风险行为。同时在【过滤条件】中限定【应用程序包含】-【explorer.exe】和【操作类型】-【删除】

    <figure><img src="../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>
*   右键征兆报表组，创建征兆报表\


    <figure><img src="../../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>
* 选择【标准征兆事件统计表】创建，条件设置选择【1分钟内删除文件超过50个】，并且由于只选择了一个征兆条件，故统计设置中，统计类型选择【计算机+征兆级别统计】即可，如果有多个统计条件，则可以勾选【按征兆类型+征兆级别】或【计算机\用户+征兆类型】进行统计
*   周期选择【标准日】\


    <figure><img src="../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>
*   配置邮件报告，首先配置SMTP，回到控制台主页，选择【工具】-【选项】-【邮件报告服务器设置】\


    <figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
*   设置好SMTP之后，回到报表控制台，上方菜单栏选择【报表】-【邮件报告】，然后以此设置收件人地址，邮件标题，以及要发送的报表\


    <figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

***

## 暂时先到这，有需要补充的联系我
