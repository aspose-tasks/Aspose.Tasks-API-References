---
title: "WorkUnit"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示工作时间。"
type: docs
weight: 362
url: /zh/java/com.aspose.tasks/workunit/
---

**Inheritance:**
java.lang.Object
```
public class WorkUnit
```

表示工作时间。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [WorkUnit(Date from, Date to)](#WorkUnit-java.util.Date-java.util.Date-) | 初始化 [WorkUnit](../../com.aspose.tasks/workunit) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getFrom()](#getFrom--) | 获取 From 日期。 |
| [getTo()](#getTo--) | 获取 To 日期。 |
| [getWorkingHours()](#getWorkingHours--) | 获取工作时间的持续时间。 |
| [setFrom(Date value)](#setFrom-java.util.Date-) | 设置 From 日期。 |
| [setTo(Date value)](#setTo-java.util.Date-) | 设置 To 日期。 |
| [setWorkingHours(double value)](#setWorkingHours-double-) | 设置工作时间的持续时间。 |
### WorkUnit(Date from, Date to) {#WorkUnit-java.util.Date-java.util.Date-}
```
public WorkUnit(Date from, Date to)
```


初始化 [WorkUnit](../../com.aspose.tasks/workunit) 类的新实例。使用指定的 From 和 To 日期创建新的 WorkUnit 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| from | java.util.Date | 工作时间的开始日期。 |
| to | java.util.Date | 工作时间的结束日期。 |

### getFrom() {#getFrom--}
```
public final Date getFrom()
```


获取 From 日期。

**Returns:**
java.util.Date - From 日期。
### getTo() {#getTo--}
```
public final Date getTo()
```


获取 To 日期。

**Returns:**
java.util.Date - 结束日期。
### getWorkingHours() {#getWorkingHours--}
```
public final double getWorkingHours()
```


获取工作时间的持续时间。

**Returns:**
double - 工作时长。
### setFrom(Date value) {#setFrom-java.util.Date-}
```
public void setFrom(Date value)
```


设置 From 日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 起始日期。 |

### setTo(Date value) {#setTo-java.util.Date-}
```
public final void setTo(Date value)
```


设置 To 日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 结束日期。 |

### setWorkingHours(double value) {#setWorkingHours-double-}
```
public final void setWorkingHours(double value)
```


设置工作时间的持续时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 工作时长。 |

