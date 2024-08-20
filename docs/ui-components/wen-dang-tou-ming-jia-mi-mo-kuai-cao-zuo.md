# 🔐 文档透明加密模块操作

加密模块UI说明

在控制台主页上有三个部分可以用于设置和加密相关的策略和配置

1. 客户端加密权限设置位置

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption><p>此处设置客户端策略</p></figcaption></figure>

2. 加密基础设置、加密相关日志及扫描加解密功能

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>此处进入文档安全的整体管理</p></figcaption></figure>

3. 解密审批流程设置

<figure><img src="../../.gitbook/assets/image (2) (1).png" alt=""><figcaption><p>此处进入审批流程设置</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3) (1).png" alt=""><figcaption><p>此处设置审批账户</p></figcaption></figure>



## 客户端加密权限设置

#### 常规设置

1. 赋予直接解密权限，并可限制直接解密数量和范围

<figure><img src="../../.gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>

2. 申请解密权限可以限制申请的文件类型及文件安全区域

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

3. 申请外发文件可以限制外发时的权限基准

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

4. 直接外发文件也可限制外发时的权限基准

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

5. 允许提取已转换成OEAX外发格式内的文件

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

6. 允许申请或直接修改文档属性（修改文件安全区域）

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

7. 允许登录审批管理平台，只有登陆了审批管理平台才能执行审批解密申请等动作

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>



***



#### 授权软件设置

1. 授权软件分为三种操作系统对应不同的授权软件，windows支持四种加密模式，四种权限限制

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
需要注意的是：禁止截屏后，任何<mark style="color:red;">已打开的授权软件</mark>均会导致截屏时黑屏；禁止复制粘贴后，仅是禁止了授权软件到<mark style="color:red;">非授权软件</mark>之间的复制粘贴，授权软件之间的复制粘贴还是正常的。
{% endhint %}

{% hint style="info" %}
四种加密模式：

自动加解密（windows/mac/linux）授权软件编辑保存文件后都会自动加密上，加密文件类型为授权库中的文件类型

智能加解密（windows/mac）只支持office文件，不含PDF，文件不会因保存动作而加密，同时也能打开加密文件，自己产生的及原来是明文的文件编辑保存后也依旧是明文状态

只读加密（windows）只支持office文件、PDF文件、图片文件，如字面意思，对加密文件只有只读的权限，打开后无法修改无法保存，自己也不会产生任何加密文件

只解密不加密（windows/mac/linux）与自动加解密相反，编辑保存文件后都会自动解密，只要是能打开的加密文件编辑保存后都会解密，一般给高层领导使用
{% endhint %}

`授权库制作方式`



***



#### 安全区域设置&文档默认安全属性

1. 安全区域分为横向和纵向两个方向，如图左侧为横向，可自己设置，右侧为纵向，系统设置

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

