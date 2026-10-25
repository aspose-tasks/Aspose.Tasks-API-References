---
title: "WeekDay"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示一个工作日，可定义一周的常规天数或日历中的例外天数。"
type: docs
weight: 352
url: /zh/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

表示一个工作日，可定义一周的常规天数或日历中的例外天数。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | 使用指定的天类型初始化 [WeekDay](../../com.aspose.tasks/weekday) 类的新实例。 |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | 使用指定的天类型和工作时间段列表初始化 [WeekDay](../../com.aspose.tasks/weekday) 类的新实例。 |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | 使用指定的天类型和工作时间段初始化 [WeekDay](../../com.aspose.tasks/weekday) 类的新实例。 |
| [WeekDay()](#WeekDay--) | 初始化 [WeekDay](../../com.aspose.tasks/weekday) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | 将 .Net 的 [DayOfWeek](../../com.aspose.tasks/dayofweek) 转换为 `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-))。 |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | 创建默认工作日。 |
| [deepClone()](#deepClone--) | 返回星期的深拷贝。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getDayType()](#getDayType--) | 获取一天的类型。 |
| [getDayWorking()](#getDayWorking--) | 获取指示指定日期或天类型是否为工作日的值。 |
| [getFromDate()](#getFromDate--) | 获取例外时间的开始。 |
| [getToDate()](#getToDate--) | 获取例外时间的结束。 |
| [getWorkingTime()](#getWorkingTime--) | 返回星期的工作时间。 |
| [getWorkingTimes()](#getWorkingTimes--) | 获取此 WeekDay 实例的 WorkingTimeCollection。 |
| [hashCode()](#hashCode--) | 返回 [WeekDay](../../com.aspose.tasks/weekday) 类实例的哈希码值。 |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | 设置一个值，指示指定的日期或日期类型是否为工作日。 |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | 为指定的星期几设置默认时间段。 |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | 设置例外时间的开始。 |
| [setToDate(Date value)](#setToDate-java.util.Date-) | 设置例外时间的结束。 |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


使用指定的天类型初始化 [WeekDay](../../com.aspose.tasks/weekday) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dayType | int | 指定的日期类型。 |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


使用指定的天类型和工作时间段列表初始化 [WeekDay](../../com.aspose.tasks/weekday) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dayType | int | 指定的日期类型。 |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | 工作时间段的列表。 |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


使用指定的天类型和工作时间段初始化 [WeekDay](../../com.aspose.tasks/weekday) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dayType | int | 指定的日期类型。 |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | 工作时间段的数组。 |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


初始化 [WeekDay](../../com.aspose.tasks/weekday) 类的新实例。

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


将 .Net 的 [DayOfWeek](../../com.aspose.tasks/dayofweek) 转换为 `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dw | int | 要进行转换的星期几。 |

**Returns:**
int - 转换后的日期类型。
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


创建默认工作日。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dayType | int | 用于创建默认工作日的日期类型。 |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


返回星期的深拷贝。

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 用于与此实例比较的对象。 |

**Returns:**
boolean - 如果指定的对象是具有相同 FromDate、ToDate 值和 WorkingTimes 的 WeekDay，则为 **True**；否则为 **false**。
### getDayType() {#getDayType--}
```
public final int getDayType()
```


获取一天的类型。

**Returns:**
int - 日期的类型。
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


获取指示指定日期或天类型是否为工作日的值。

**Returns:**
boolean - 指示指定的日期或日期类型是否为工作日的值。
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


获取例外时间的开始。

**Returns:**
java.util.Date - 例外时间的开始。
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


获取例外时间的结束。

**Returns:**
java.util.Date - 例外时间的结束。
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


返回星期的工作时间。

**Returns:**
double - 工作时间。
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


获取此 WeekDay 实例的 WorkingTimeCollection。该集合定义了工作日的工作时间段。

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回 [WeekDay](../../com.aspose.tasks/weekday) 类实例的哈希码值。

**Returns:**
int - 返回此对象的哈希码值。
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


设置一个值，指示指定的日期或日期类型是否为工作日。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示指定的日期或日期类型是否为工作日的值。 |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


为指定的星期几设置默认时间段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | 要设置默认工作日的星期几。 |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


设置例外时间的开始。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 异常时间的开始。 |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


设置例外时间的结束。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 异常时间的结束。 |

