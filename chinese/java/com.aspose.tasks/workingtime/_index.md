---
title: "WorkingTime"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示工作日内的工作时间。"
type: docs
weight: 365
url: /zh/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

表示工作日内的工作时间。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | 使用指定的开始和结束时间的间隔，初始化 [WorkingTime](../../com.aspose.tasks/workingtime) 类的新实例。 |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | 使用指定的开始和结束时间的间隔项，初始化 [WorkingTime](../../com.aspose.tasks/workingtime) 类的新实例。 |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | 使用指定的开始和结束时间的间隔项，初始化 [WorkingTime](../../com.aspose.tasks/workingtime) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | 检查对象是否相等。 |
| [getFrom()](#getFrom--) | 获取工作时间的开始。 |
| [getTo()](#getTo--) | 获取工作时间的结束。 |
| [hashCode()](#hashCode--) | 返回 [WorkingTime](../../com.aspose.tasks/workingtime) 类实例的哈希码值。 |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


使用指定的开始和结束时间的间隔，初始化 [WorkingTime](../../com.aspose.tasks/workingtime) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fromTime | java.util.Date | 间隔开始时间 |
| toTime | java.util.Date | 间隔结束时间 |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


使用指定的开始和结束时间的间隔项，初始化 [WorkingTime](../../com.aspose.tasks/workingtime) 类的新实例。

--------------------

&gt; ```
&gt; 可以使用 WorkingTime 构造函数的重载来使用 TimeSpan 初始化间隔的开始和结束：
&gt; ``````

 [C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | double | Interval's start time represented by double struct. |
| toTime | double | Interval's end time represented by double struct. |

### WorkingTime(int fromHours, int toHours) {#WorkingTime-int-int-}
```
public WorkingTime(int fromHours, int toHours)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times.

--------------------

&gt; ```
&gt; The overload of WorkingTime ctor can be used to initialize interval's start and end using whole hours:
&gt; ``````

 [C#]
 var wt = new WorkingTime(9, 13);
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fromHours | int | 间隔的开始时间，以整数小时表示（0-24）。 |
| toHours | int | 间隔的结束时间，以整数小时表示（0-24）。 |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


检查对象是否相等。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 第二个待比较的对象。 |

**Returns:**
boolean - 如果对象相等则为 True，否则为 false。
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


获取工作时间的开始。

**Returns:**
java.util.Date - 工作时间的开始。
### getTo() {#getTo--}
```
public final Date getTo()
```


获取工作时间的结束。

**Returns:**
java.util.Date - 工作时间的结束。
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回 [WorkingTime](../../com.aspose.tasks/workingtime) 类实例的哈希码值。

**Returns:**
int - 返回此对象的哈希码值。
