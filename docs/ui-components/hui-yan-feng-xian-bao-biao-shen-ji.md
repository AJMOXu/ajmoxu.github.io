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

## 报表UI说明

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


    <figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
* 用于评估内网的平均上传大小，获取到合适的数据用于【征兆表】的创建

#### 如何创建趋势表

*   右键报表分组，新建报表，选择【从查询条件创建】\


    <figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
*   选择需要创建的趋势表，例如这里我想筛选文档操作相关的日志，就选【标准文档操作趋势表】\


    <figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>
*   筛选感兴趣的日志，例如截图中筛选的是所有删除用户手动删除的日志。然后点击【下一步】\


    <figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
*   选择统计单位（时间间隔，最短一天）和统计类型（统计用户的行为，还是计算机行为）然后【下一步】\


    <figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>
*   选择报表统计的周期时间，这里选择【标准月】即可，然后【下一步】\


    <figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>
*   命名报表名称，然后点击【完成】\


    <figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
*   创建后不会自动立即统计过往数据，需要到【报表】-【生成历史报表】-选择刚创建的报表-选择生成的时间范围，保存后才能开始统计过往数据（统计需要时间）\


    <figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

***



### 统计表

#### 统计表用途场景

*   用于直观的看到一段时间内的各项数据的总数据大小，例如图中展示的是2024年11月的删除、上传、下载文件数量和大小

    <figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>
*   结合【资产管理模块】，统计内网软硬件资产\


    <figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

#### 创建统计表（与趋势表一样）

*   右键报表分组，新建报表，选择【从查询条件创建】

    <figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>
*   根据需要选择对应模块报表，这里依旧选择【文档操作报表】\


    <figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>
* 之后的操作和趋势表一样，这里就不再补充了，如果需要补充请联系我

***
