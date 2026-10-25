---
title: "费率"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示资源在该时间段内适用的时间段定义和费率。"
type: docs
weight: 232
url: /zh/java/com.aspose.tasks/rate/
---

**Inheritance:**
java.lang.Object
```
public class Rate
```

表示资源在该时间段内适用的时间段定义和费率。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCostPerUse()](#getCostPerUse--) | 获取资源的每次使用费用。 |
| [getOvertimeRate()](#getOvertimeRate--) | 获取资源每小时的加班费率。 |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | 获取 Microsoft Project 用于显示加班费率的单位。 |
| [getRateTable()](#getRateTable--) | 获取资源费率表的唯一标识符。 |
| [getRatesFrom()](#getRatesFrom--) | 获取费率生效的日期。 |
| [getRatesTo()](#getRatesTo--) | 获取费率最后生效的日期。 |
| [getStandardRate()](#getStandardRate--) | 获取资源每小时的标准费率。 |
| [getStandardRateFormat()](#getStandardRateFormat--) | 获取 Microsoft Project 用于显示标准费率的单位。 |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | 设置资源的每次使用成本。 |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | 设置资源的每小时加班费率。 |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | 设置 Microsoft Project 用于显示加班费率的单位。 |
| [setRateTable(int value)](#setRateTable-int-) | 设置资源的费率表唯一标识符。 |
| [setRatesFrom(Date value)](#setRatesFrom-java.util.Date-) | 设置费率生效的日期。 |
| [setRatesTo(Date value)](#setRatesTo-java.util.Date-) | 设置费率有效的最后日期。 |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | 设置资源的每小时标准费率。 |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | 设置 Microsoft Project 用于显示标准费率的单位。 |
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


获取资源的每次使用成本。如果资源存在费率表，则从当前日期检索此值。

**Returns:**
java.math.BigDecimal - 资源的每次使用成本。
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


获取资源每小时的加班费率。

**Returns:**
java.math.BigDecimal - 资源的每小时加班费率。
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


获取 Microsoft Project 用于显示加班费率的单位。

**Returns:**
int - Microsoft Project 用于显示加班费率的单位。
### getRateTable() {#getRateTable--}
```
public final int getRateTable()
```


获取资源费率表的唯一标识符。

**Returns:**
int - 资源的费率表唯一标识符。
### getRatesFrom() {#getRatesFrom--}
```
public final Date getRatesFrom()
```


获取费率生效的日期。

**Returns:**
java.util.Date - 费率生效的日期。
### getRatesTo() {#getRatesTo--}
```
public final Date getRatesTo()
```


获取费率最后生效的日期。

**Returns:**
java.util.Date - 费率有效的最后日期。
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


获取资源每小时的标准费率。

**Returns:**
java.math.BigDecimal - 资源的每小时标准费率。
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


获取 Microsoft Project 用于显示标准费率的单位。

**Returns:**
int - Microsoft Project 用于显示标准费率的单位。
### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


设置资源的每次使用成本。如果资源存在费率表，则从当前日期检索此值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | 资源的每次使用成本。 |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


设置资源的每小时加班费率。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | 资源的每小时加班费率。 |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


设置 Microsoft Project 用于显示加班费率的单位。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | Microsoft Project 用于显示加班费率的单位。 |

### setRateTable(int value) {#setRateTable-int-}
```
public final void setRateTable(int value)
```


设置资源的费率表唯一标识符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 资源的费率表唯一标识符。 |

### setRatesFrom(Date value) {#setRatesFrom-java.util.Date-}
```
public final void setRatesFrom(Date value)
```


设置费率生效的日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 费率生效的日期。 |

### setRatesTo(Date value) {#setRatesTo-java.util.Date-}
```
public final void setRatesTo(Date value)
```


设置费率有效的最后日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 费率有效的最后日期。 |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


设置资源的每小时标准费率。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | 资源的每小时标准费率。 |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


设置 Microsoft Project 用于显示标准费率的单位。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | Microsoft Project 用于显示标准费率的单位。 |

