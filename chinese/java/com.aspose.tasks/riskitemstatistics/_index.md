---
title: "RiskItemStatistics"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示存储已分析项目任务统计数据的项。"
type: docs
weight: 265
url: /zh/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

表示存储已分析项目任务统计数据的项。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | 获取风险项的期望值。 |
| [getItemType()](#getItemType--) | 获取 [RiskItemType](../../com.aspose.tasks/riskitemtype) 枚举的实例。 |
| [getMaximum()](#getMaximum--) | 获取在蒙特卡罗模拟期间生成的最大值。 |
| [getMinimum()](#getMinimum--) | 获取在蒙特卡罗模拟期间生成的最小值。 |
| [getPercentile(int percent)](#getPercentile-int-) | 获取一个阈值，使得指定百分比的生成样本低于该值。 |
| [getStandardDeviation()](#getStandardDeviation--) | 获取风险项的标准偏差。 |
| [toString()](#toString--) | 返回风险项的简短字符串表示。 |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


获取风险项的期望值。

**Returns:**
java.util.Date - 风险项的期望值。
### getItemType() {#getItemType--}
```
public final int getItemType()
```


获取 [RiskItemType](../../com.aspose.tasks/riskitemtype) 枚举的实例。

**Returns:**
int - [RiskItemType](../../com.aspose.tasks/riskitemtype) 枚举的实例。
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


获取在蒙特卡罗模拟期间生成的最大值。

**Returns:**
java.util.Date - 在蒙特卡罗模拟期间生成的最大值。
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


获取在蒙特卡罗模拟期间生成的最小值。

**Returns:**
java.util.Date - 在蒙特卡罗模拟期间生成的最小值。
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


获取一个阈值，使得指定百分比的生成样本低于该值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 百分比 | int | 0 到 100 之间的指定百分比。 |

**Returns:**
java.util.Date - 一个阈值，使得指定百分比的生成样本低于该值。
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


获取风险项的标准偏差。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


返回风险项的简短字符串表示。表示的具体细节未指定，且可能会更改。

**Returns:**
java.lang.String - 表示 RiskItem 对象的简短字符串。
