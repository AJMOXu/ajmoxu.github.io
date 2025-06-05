---
icon: sistrix
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

# 敏感信息识别

## 前言：

{% hint style="info" %}
敏感内容识别，非常依赖于<mark style="color:red;">**敏感信息分类库**</mark>，因此<mark style="color:red;">**建立敏感信息库是重中之重**</mark>。
{% endhint %}

***

## 建立敏感信息库

### 根据行业区分

{% tabs %}
{% tab title="制造业" %}
制造业以BOM表单、研发资料、采购订单、合同订单、项目协议等信息为主，因此可以着重抓取以下几个维度的信息

* <mark style="color:red;">**BOM表单**</mark>：物料编码/型号规格/采购代码/项目编码/BOM单号/ERP单号
* <mark style="color:red;">**工程需求单**</mark>：物料编码/规格参数/项目编码/工程单号/EC编号/ECN ECR编号/图纸编号
* <mark style="color:red;">**研发资料-3D转PDF图纸**</mark>：规格参数(含单位)/图纸描述/图纸编码/公司名称/签名名称/图纸尺寸(含单位)
* <mark style="color:red;">**研发资料-项目方案(项目协议)**</mark>：高频词汇/项目编号/组件名称/工艺技术要求(含具体单位)/设备技术要求(含具体指标)
* <mark style="color:red;">**产品测试报告**</mark>：CAS号码/测试项目/测试名称/测试结果(含具体数值，如百分比)
* <mark style="color:red;">**合同订单**</mark>：销售协议高频词汇/合同编码/公司名称/合同金额
{% endtab %}

{% tab title="金融业" %}

{% endtab %}

{% tab title="电商行业" %}

{% endtab %}
{% endtabs %}

### AI分析敏感信息

目前的流程是：

1. 收集敏感信息，统计到表格
2. 将智能体提示词输入给AI，再将统计后的表格发送给AI
3. 将AI输出的正则表达式内容，输入到系统的敏感内容分类库中

{% hint style="info" %}
智能体提示词（目前支持deepseek）：
{% endhint %}

> I want you to act as a cyber security specialist. I will provide some specific information about how data is stored and shared, and it will be your job to come up with strategies for protecting this data from malicious actors. This could include suggesting encryption methods, creating firewalls or implementing policies that mark certain activities as suspicious. Additionally, I am highly proficient in file DLP functionality and adept at generating regular expressions based on file samples. When creating regular expressions, I can adjust patterns per reasonable requirements or industry standards to ensure precise identification and minimize false positives. I also meticulously calculate the weight ratio for each sensitive keyword, ensuring a balanced allocation that prevents misidentification.\
> You will receive sensitive information statistics primarily presented in tables. The first row of each column contains the header, indicating the type of sensitive information for that column. The rows below the headers contain the detailed content of this sensitive information. Importantly: Starting from the second column (Column B), calculate regular expressions based on the sensitive information. The first column (Column A) serves as an example and should not be calculated.

{% hint style="info" %}
敏感信息统计表
{% endhint %}

{% file src="../../.gitbook/assets/敏感信息统计表.xlsx" %}

