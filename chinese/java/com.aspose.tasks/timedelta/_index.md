---
title: "TimeDelta"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示两个时间戳之间的差异。"
type: docs
weight: 317
url: /zh/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

表示两个时间戳之间的差异。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | 将 TimeDelta 初始化为指定的小时、分钟和秒数的新实例。 |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | 将 TimeDelta 初始化为指定的天、小时、分钟、秒和毫秒数的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | 返回一个新的 TimeDelta 对象，其值为此实例与另一个实例的和。 |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | 比较两个 TimeDelta 值，并返回一个整数，指示第一个值是短于、等于还是长于第二个值。 |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | 将此实例与指定的 TimeDelta 对象进行比较，并返回一个整数，指示此实例是短于、等于还是长于 TimeSpan 对象。 |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | 指示某个 `other` 时间跨度是否等于此时间跨度。 |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | 检查两个实例是否相等。 |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | 返回一个表示指定天数（四舍五入到最近的毫秒）的 TimeDelta。 |
| [fromHours(double value)](#fromHours-double-) | 返回一个表示指定小时数（四舍五入到最近的毫秒）的 TimeDelta。 |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | 返回一个表示指定毫秒数（四舍五入到最近的毫秒）的 TimeDelta。 |
| [fromMinutes(double value)](#fromMinutes-double-) | 返回一个表示指定分钟数（四舍五入到最近的毫秒）的 TimeDelta。 |
| [fromSeconds(double value)](#fromSeconds-double-) | 返回一个表示指定秒数（四舍五入到最近的毫秒）的 TimeDelta。 |
| [getDays()](#getDays--) | 返回此实例表示的时间间隔的天数部分。 |
| [getHours()](#getHours--) | 返回此实例表示的时间间隔的小时部分。 |
| [getMilliseconds()](#getMilliseconds--) | 返回此实例表示的时间间隔的毫秒部分。 |
| [getMinutes()](#getMinutes--) | 返回此实例表示的时间间隔的分钟组件。 |
| [getSeconds()](#getSeconds--) | 返回此实例表示的时间间隔的秒组件。 |
| [getTotalDays()](#getTotalDays--) | 返回当前实例以整数和小数天表示的值。 |
| [getTotalHours()](#getTotalHours--) | 返回当前实例以整数和小数小时表示的值。 |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | 返回当前实例以整数和小数毫秒表示的值。 |
| [getTotalMinutes()](#getTotalMinutes--) | 返回当前实例以整数和小数分钟表示的值。 |
| [getTotalSeconds()](#getTotalSeconds--) | 返回当前实例以整数和小数秒表示的值。 |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | 返回一个新的 `TimeDelta`，其值为此实例的相反数。 |
| [parse(String s)](#parse-java.lang.String-) | 将时间间隔的字符串表示转换为其 `TimeDelta` 等价物。 |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | 返回一个新的 TimeDelta 对象，其值为此实例与 `other` 实例之间的差值。 |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | 将时间间隔的字符串表示转换为其 TimeDelta 等价物，并返回一个指示转换是否成功的值。 |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


将 TimeDelta 初始化为指定的小时、分钟和秒数的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 小时 | int | 小时数。 |
| 分钟 | int | 分钟数。 |
| 秒 | int | 秒数。 |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


将 TimeDelta 初始化为指定的天、小时、分钟、秒和毫秒数的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 天 | int | 天数。 |
| 小时 | int | 小时数。 |
| 分钟 | int | 分钟数。 |
| 秒 | int | 秒数。 |
| 毫秒 | int | 毫秒数。 |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


返回一个新的 TimeDelta 对象，其值为此实例与另一个实例的和。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | 要相加的实例。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance plus value of other instance.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### compare(TimeDelta t1, TimeDelta t2) {#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static int compare(TimeDelta t1, TimeDelta t2)
```


比较两个 TimeDelta 值，并返回一个整数，指示第一个值是短于、等于还是长于第二个值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | 要比较的第一个时间间隔。 |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | 要比较的第二个时间间隔。 |

**Returns:**
int - \-1 如果 `t1` 短于 `t2`，0 如果 `t1` 等于 `t2`，以及 1 如果 `t1` 长于 `t2`。
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


将此实例与指定的 TimeDelta 对象进行比较，并返回一个整数，指示此实例是短于、等于还是长于 TimeSpan 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | 用于比较的实例。 |

**Returns:**
int - \-1 如果此实例比 `other` 短，0 如果此实例等于 `other`，并且 1 如果此实例比 `other` 长。
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


指示某个 `other` 时间跨度是否等于此时间跨度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | 用于比较的时间跨度。 |

**Returns:**
boolean - `true` 如果区间相等；`false` 否则。
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


检查两个实例是否相等。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | 第一个实例。 |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | 第二个实例。 |

**Returns:**
boolean - `true` 如果实例相等；`false` 否则。
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 其他 | java.lang.Object | \{@inheritDoc\} |

**Returns:**
布尔 - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


返回一个表示指定天数（四舍五入到最近的毫秒）的 TimeDelta。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 天数。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


返回一个表示指定小时数（四舍五入到最近的毫秒）的 TimeDelta。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 小时数。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


返回一个表示指定毫秒数（四舍五入到最近的毫秒）的 TimeDelta。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 毫秒数。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


返回一个表示指定分钟数（四舍五入到最近的毫秒）的 TimeDelta。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 分钟数。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


返回一个表示指定秒数（四舍五入到最近的毫秒）的 TimeDelta。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 秒数。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


返回此实例表示的时间间隔的天数部分。

**Returns:**
int - 时间间隔的天数部分。可以是正数或负数。
### getHours() {#getHours--}
```
public int getHours()
```


返回此实例表示的时间间隔的小时部分。

**Returns:**
int - 时间间隔的小时部分，范围从 -23 到 23。
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


返回此实例表示的时间间隔的毫秒部分。

**Returns:**
int - 时间间隔的毫秒部分，范围从 -999 到 999。
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


返回此实例表示的时间间隔的分钟组件。

**Returns:**
int - 时间间隔的分钟部分，范围从 -59 到 59。
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


返回此实例表示的时间间隔的秒组件。

**Returns:**
int - 时间间隔的秒数部分，范围从 -59 到 59。
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


返回当前实例以整数和小数天表示的值。

**Returns:**
double - 此实例表示的天数总计。
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


返回当前实例以整数和小数小时表示的值。

**Returns:**
double - 此实例表示的小时总计。
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


返回当前实例以整数和小数毫秒表示的值。

**Returns:**
double - 此实例表示的毫秒总计。
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


返回当前实例以整数和小数分钟表示的值。

**Returns:**
double - 此实例表示的分钟总计。
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


返回当前实例以整数和小数秒表示的值。

**Returns:**
double - 此实例表示的秒数总计。
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int - \{@inheritDoc\}
### negate() {#negate--}
```
public TimeDelta negate()
```


返回一个新的 `TimeDelta`，其值为此实例的相反数。

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


将时间间隔的字符串表示转换为其 `TimeDelta` 等价物。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| s | java.lang.String | 指定要转换的时间间隔的字符串。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


返回一个新的 TimeDelta 对象，其值为此实例与 `other` 实例之间的差值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | 要减去的实例。 |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance minus value of other instance.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String - \{@inheritDoc\}
### tryParse(String s, TimeDelta[] result) {#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---}
```
public static boolean tryParse(String s, TimeDelta[] result)
```


将时间间隔的字符串表示转换为其 TimeDelta 等价物，并返回一个指示转换是否成功的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| s | java.lang.String | 指定要转换的时间间隔的字符串。 |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | 此数组必须至少包含一个元素。当此方法返回时，`result[0]` 包含一个对象，该对象表示由 `s` 指定的时间间隔；如果转换失败，则为零长度时间间隔。 |

**Returns:**
boolean - 如果 s 转换成功，则为 `true`；否则为 `false`。
