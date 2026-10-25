---
title: "AvailabilityPeriod"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示资源可用的时间段。"
type: docs
weight: 20
url: /zh/java/com.aspose.tasks/availabilityperiod/
---

**Inheritance:**
java.lang.Object
```
public class AvailabilityPeriod
```

表示资源可用的时间段。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AvailabilityPeriod()](#AvailabilityPeriod--) | 初始化一个新的 [AvailabilityPeriod](../../com.aspose.tasks/availabilityperiod) 实例。 |
| [AvailabilityPeriod(Date availableFrom, Date availableTo, double availableUnits)](#AvailabilityPeriod-java.util.Date-java.util.Date-double-) | 使用指定的日期范围和可用单位初始化一个新的 [AvailabilityPeriod](../../com.aspose.tasks/availabilityperiod) 实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getAvailableFrom()](#getAvailableFrom--) | 获取资源在指定期间可用的日期。 |
| [getAvailableTo()](#getAvailableTo--) | 获取资源在指定期间可用的最后日期。 |
| [getAvailableUnits()](#getAvailableUnits--) | 获取资源在指定期间的可用百分比。 |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | 设置资源在指定期间可用的日期。 |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | 设置资源在指定期间可用的最后日期。 |
| [setAvailableUnits(double value)](#setAvailableUnits-double-) | 设置在指定期间内资源可用的百分比。 |
### AvailabilityPeriod() {#AvailabilityPeriod--}
```
public AvailabilityPeriod()
```


初始化一个新的 [AvailabilityPeriod](../../com.aspose.tasks/availabilityperiod) 实例。

### AvailabilityPeriod(Date availableFrom, Date availableTo, double availableUnits) {#AvailabilityPeriod-java.util.Date-java.util.Date-double-}
```
public AvailabilityPeriod(Date availableFrom, Date availableTo, double availableUnits)
```


使用指定的日期范围和可用单位初始化一个新的 [AvailabilityPeriod](../../com.aspose.tasks/availabilityperiod) 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| availableFrom | java.util.Date | 起始日期 |
| availableTo | java.util.Date | 结束日期 |
| availableUnits | double | 可用单位 |

### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


获取资源在指定期间可用的日期。

**Returns:**
java.util.Date - 资源在指定期间开始可用的日期。
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


获取资源在指定期间可用的最后日期。

**Returns:**
java.util.Date - 资源在指定期间最后可用的日期。
### getAvailableUnits() {#getAvailableUnits--}
```
public final double getAvailableUnits()
```


获取资源在指定期间的可用百分比。

**Returns:**
double - 在指定期间内资源可用的百分比。
### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


设置资源在指定期间可用的日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 资源在指定期间开始可用的日期。 |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


设置资源在指定期间可用的最后日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 资源在指定期间最后可用的日期。 |

### setAvailableUnits(double value) {#setAvailableUnits-double-}
```
public final void setAvailableUnits(double value)
```


设置在指定期间内资源可用的百分比。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 资源在指定期间可用的百分比。 |

