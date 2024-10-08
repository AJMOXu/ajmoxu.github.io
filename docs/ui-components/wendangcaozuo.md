---
title: 文档操作
parent: IP-Guard
nav_order: 5
icon: file-magnifying-glass
---

# 文档操作

## 策略设置面板的各项属性

在高级->文档操作管控中找到策略设置界面

* **操作类型**：为了方便理解和控制，把文档操作类型简单的分为：读取、修改、删除这 3 种。其中，允许修改就一定可以读取，允许删除就一定可以读取和修改
* **盘符类型**：默认是全部盘符类型，至少要选择一种盘符类型，否则自动识别为全部。选中“盘符类型”，可以用 Ctrl + A 对其所有子项进行全选或全不选
* **文件名称**：指定需要控制的文件名称，可以包含路径，如E:\work\*，则 work 这个文件夹下的所有文件都生效。文件名称支持通配符，支持“;”“,”作为分隔符
* **修改前备份**：备份修改的文件，只会备份修改之前的源文件，以防止重要文件被恶意或无意修改
* **复制/移动到备份**：复制/移动到指定盘符类型时备份文件，方便检查客户端机器是否将重要文件复制/移动到非法的盘符
* **复制/移动出备份**：复制/移动出指定盘符类型时备份文件，方便检查客户端机器是否将重要盘符内的文件复制/移动到其他盘符
* **删除前备份**：备份客户端删除的文件，避免重要资料被误删除而带来的损失
* **应用程序**：指定文档操作的应用程序
*   PS：文档操作策略中，盘符类型选择“光盘”时，只针对使用专用刻录工具进行刻录操作生效。&#x20;

    <figure><img src="https://user-images.githubusercontent.com/123937106/218038484-c1428e6a-d271-4d7f-9a22-f90690bc9a9a.png" alt=""><figcaption></figcaption></figure>

## 文档操作策略设置

文档操作策略可以灵活多变，但如果设置不谨慎将会导致严重问题

策略示例：

*   管辖范围内的所有客户端主动删除文件时，均会将文件备份到服务器&#x20;

    <figure><img src="https://user-images.githubusercontent.com/123937106/218041633-433e38ae-5d9e-4565-a8ac-a7f23a0f322d.png" alt=""><figcaption></figcaption></figure>

策略示例：

* 管辖范围内的所有客户端，对\192.168.100.100\设计图纸\ 与 \192.168.100.100\项目代码\ 目录下的文件及文件夹仅有读取权限

<div align="center">

<figure><img src="https://user-images.githubusercontent.com/123937106/218042114-b22d999d-fd30-42fd-91e2-b600545865e5.png" alt=""><figcaption></figcaption></figure>

</div>

策略示例：

*   管辖范围内的所有客户端，禁止对所有可移动盘写入文件或修改删除可移动盘文件&#x20;

    <figure><img src="https://user-images.githubusercontent.com/123937106/218042615-56e25446-07ce-41b8-a324-fa3c6542bbd0.png" alt=""><figcaption></figcaption></figure>

策略示例：

*   管辖范围内的所有客户端，禁止使用浏览器下载文件（多数浏览器在下载文件时会先创建.download缓存文件，有些后缀可能有些不一样但基本大差不差）\
    &#x20;

    <figure><img src="https://user-images.githubusercontent.com/123937106/218042969-0756eb94-f1c8-4278-a127-1893e8576436.png" alt=""><figcaption></figcaption></figure>

## 文档操作日志查询

在日志->文档操作中找到文档操作对应的日志

<figure><img src="https://user-images.githubusercontent.com/123937106/218043915-bb843230-ffa4-4539-9455-bdc6f9ea3bd6.png" alt=""><figcaption></figcaption></figure>

文档操作日志的内容很多很杂，很多后台进程的操作行为也会被记录下来，要想筛选到有价值的数据，需要熟练使用右边的筛查项；或将所有日志导出为csv格式后使用excel进行数据处理

筛查项示例：

*   查询所有网页上传文件的行为\
    &#x20;

    <figure><img src="https://user-images.githubusercontent.com/123937106/218044421-f703d79c-8574-45a6-9c34-925d8c454c12.png" alt=""><figcaption></figcaption></figure>
*   查询所有拷贝到U盘的行为（由于我这边是虚拟机，没有用过U盘，所以没有日志）&#x20;

    <figure><img src="https://user-images.githubusercontent.com/123937106/218044614-a380b9ec-a40d-4219-8746-439e5c91f0ed.png" alt=""><figcaption></figcaption></figure>
*   查询某个类型的文件的重命名操作\
    &#x20;

    <figure><img src="https://user-images.githubusercontent.com/123937106/218044879-96018e88-c878-4991-8bb5-cd201d071fdf.png" alt=""><figcaption></figcaption></figure>
*   导出筛选出的数据（所有满足条件的记录即除了当页之外，筛查器筛查出来的所有日志）&#x20;

    <figure><img src="https://user-images.githubusercontent.com/123937106/218045099-7201d035-9ae8-49d7-bde5-e64a4794a96f.png" alt=""><figcaption></figcaption></figure>

## 文档操作联动功能

文档操作模块目前可联动屏幕记录与水印追溯 策略示例：

* 管辖范围内所有客户端删除文件时自动进行屏幕追踪记录（2s一次，一共3次）
* 需要2个策略配合使用才可做到

1.  读取和修改不记录屏幕\


    <figure><img src="https://user-images.githubusercontent.com/123937106/218046541-9d47372c-f627-495a-9ff6-812ad60cea49.png" alt=""><figcaption></figcaption></figure>
2.  读取和修改被前面一条策略覆盖了，仅有删除会匹配到屏幕记录策略

    <figure><img src="https://user-images.githubusercontent.com/123937106/218046720-a324c3c2-3ca4-4ec4-937a-7849c3fddb07.png" alt=""><figcaption></figcaption></figure>

策略示例：

* 管辖范围内所有客户端拷贝office、pdf、图像文件到U盘时，自动对文件打上水印
*   管辖范围内所有客户端上传office、pdf、图像文件到网络盘时，自动对文件打上水印&#x20;

    <figure><img src="https://user-images.githubusercontent.com/123937106/218047670-3dcf57a2-9767-4fe5-9254-6cf69581abf6.png" alt=""><figcaption></figcaption></figure>
