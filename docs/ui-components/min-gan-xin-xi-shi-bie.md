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
