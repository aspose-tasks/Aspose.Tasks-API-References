---
title: "Duration"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示项目中的持续时间。"
type: docs
weight: 76
url: /zh/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

表示项目中的持续时间。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Duration()](#Duration--) | 使用指定的 TimeSpan 值和 TimeUnitType 初始化 [Duration](../../com.aspose.tasks/duration) 结构的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [Clone()](#Clone--) | 创建并返回此实例的深拷贝。 |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | 将实例的深拷贝复制到另一个实例。 |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | 将指定的持续时间添加到此持续时间。 |
| [add(double val)](#add-double-) | 将指定的 double 值添加到此持续时间。 |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | 将 Duration 对象转换为具有指定时间单位的其他持续时间。 |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | 返回一个值，指示指定的 `obj1` 实例是否等于指定的 `obj2` 实例。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getTimeSpan()](#getTimeSpan--) | 获取此 Duration 对象的 `TimeSpan`（[getTimeSpan](../../com.aspose.tasks/duration\\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\\#setTimeSpan-TimeSpan-)）实例。 |
| [getTimeUnit()](#getTimeUnit--) | 获取此对象的时间单位类型。 |
| [hashCode()](#hashCode--) | 返回此对象的哈希码值。 |
| [isElapsed()](#isElapsed--) | 获取指示时间单位是否已过去的值。 |
| [isEstimated()](#isEstimated--) | 获取指示时间单位是否为估计的值。 |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | 返回一个值，指示此实例是否不等于指定的对象。 |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | 将指定的字符串转换为 [Duration](../../com.aspose.tasks/duration) 结构的实例。 |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | 解析格式为 "PT--H--M--S--" 的持续时间字符串。 |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | 从此持续时间实例中减去指定的持续时间。 |
| [subtract(double val)](#subtract-double-) | 从此持续时间实例中减去指定的 double 值。 |
| [toDouble()](#toDouble--) | 将 Duration 对象转换为 `double` 值。 |
| [toString()](#toString--) | 返回此实例的字符串表示形式。 |
### Duration() {#Duration--}
```
public Duration()
```


使用指定的 TimeSpan 值和 TimeUnitType 初始化 [Duration](../../com.aspose.tasks/duration) 结构的新实例。

### Clone() {#Clone--}
```
public Duration Clone()
```


创建并返回此实例的深拷贝。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


将实例的深拷贝复制到另一个实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | 另一个实例。 |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


将指定的持续时间添加到此持续时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | 指定要添加到此实例的 [Duration](../../com.aspose.tasks/duration)。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


将指定的 double 值添加到此持续时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| val | double | 指定要添加到此实例的 `double` 值。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### convert(byte timeUnitType) {#convert-byte-}
```
public final Duration convert(byte timeUnitType)
```


将 Duration 对象转换为具有指定时间单位的其他持续时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| timeUnitType | 字节 | 指定的时间单位类型。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | 用于与此实例比较的对象。 |

**Returns:**
布尔型 - 如果其他 Duration 实例具有与此实例相同的 TimeSpan 和 TimeUnit 值，则返回 **True**；否则返回 **false**。
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


返回一个值，指示指定的 `obj1` 实例是否等于指定的 `obj2` 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | 要比较的第一个对象。 |
| obj2 | [Duration](../../com.aspose.tasks/duration) | 要比较的第二个对象。 |

**Returns:**
boolean - 如果指定的 `obj1` 实例等于指定的 `obj2` 实例则返回 true；否则返回 false。
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
布尔型 - 如果指定的对象是具有与此实例相同的 TimeSpan 和 TimeUnit 值的 Duration，则为 **True**；否则为 **false**。
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


获取此 Duration 对象的 `TimeSpan`（[getTimeSpan](../../com.aspose.tasks/duration\\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\\#setTimeSpan-TimeSpan-)）实例。

值：此 Duration 对象的 TimeSpan 实例。

**Returns:**
double - 此 Duration 对象的 `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) 实例。
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


获取此对象的时间单位类型。

值：此 Duration 实例的时间单位类型。

**Returns:**
byte - 此对象的时间单位类型。
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回此对象的哈希码值。

**Returns:**
int - 返回此持续时间实例的哈希码值。
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


获取指示时间单位是否已过去的值。

值：确定此 Duration 实例是否已过去的标志。

**Returns:**
布尔型 - 指示时间单位是否已过去的值。
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


获取指示时间单位是否为估计的值。

值：确定此 Duration 实例是否为估计的标志。

**Returns:**
布尔型 - 指示时间单位是否为估计的值。
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | 第一个持续时间。 |
| b | [Duration](../../com.aspose.tasks/duration) | 第二个持续时间。 |

**Returns:**
boolean - 一个值，指示此实例是否等于指定的对象
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


返回一个值，指示此实例是否不等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | 第一个持续时间。 |
| b | [Duration](../../com.aspose.tasks/duration) | 第二个持续时间。 |

**Returns:**
boolean - 一个值，指示此实例是否不等于指定的对象
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


将指定的字符串转换为 [Duration](../../com.aspose.tasks/duration) 结构的实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | 指定用于转换持续时间的 [Project](../../com.aspose.tasks/project) 类实例。 |
| 值 | java.lang.String | 指定要转换的字符串。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


解析格式为 "PT--H--M--S--" 的持续时间字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 指定要解析的字符串。 |

**Returns:**
double - 返回已解析的 `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) 结构体实例。
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


从此持续时间实例中减去指定的持续时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | 指定要从此实例中减去的 [Duration](../../com.aspose.tasks/duration) 实例。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


从此持续时间实例中减去指定的 double 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| val | double | 指定要从此实例中减去的 `double` 值。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


将 Duration 对象转换为 `double` 值。

**Returns:**
double - 转换后的值。
### toString() {#toString--}
```
public String toString()
```


返回此实例的字符串表示形式。

**Returns:**
java.lang.String - 此实例的字符串表示形式。
