---
title: "TimephasedData"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示时间分段数据。"
type: docs
weight: 320
url: /zh/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

表示时间分段数据。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | 初始化 [TimephasedData](../../com.aspose.tasks/timephaseddata) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | 创建并初始化用于基于成本的时间分段数据的 [TimephasedData](../../com.aspose.tasks/timephaseddata) 类的新实例。 |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | 创建并初始化用于基于成本的时间分段数据的 [TimephasedData](../../com.aspose.tasks/timephaseddata) 类的新实例。 |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | 创建并初始化用于材料资源分配的基于单位的时间分段数据的 [TimephasedData](../../com.aspose.tasks/timephaseddata) 类的新实例。 |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | 创建并初始化用于基于工作量的时间分段数据的 [TimephasedData](../../com.aspose.tasks/timephaseddata) 类的新实例。 |
| [getFinish()](#getFinish--) | 获取时间分段数据期间的结束日期。 |
| [getStart()](#getStart--) | 获取时间分段数据期间的开始日期。 |
| [getTimephasedDataType()](#getTimephasedDataType--) | 获取时间分段数据的类型。 |
| [getUid()](#getUid--) | 获取时间分段数据的唯一标识符 |
| [getUnit()](#getUnit--) | 获取时间分段数据期间的时间单位。 |
| [getValue()](#getValue--) | 获取时间分段数据期间每时间单位的值。 |
| [getValueToCost()](#getValueToCost--) | 获取 `double` 实例，该实例表示此对象的字符串值。 |
| [getValueToDuration()](#getValueToDuration--) | 获取 double 实例，该实例表示此对象的字符串值。 |
| [getValueToUnits()](#getValueToUnits--) | 获取 `double` 实例，该实例表示基于单位的时间分段数据的字符串值。 |
| [setFinish(Date value)](#setFinish-java.util.Date-) | 设置时间分段数据期间的结束日期。 |
| [setStart(Date value)](#setStart-java.util.Date-) | 设置时间分段数据期间的开始日期。 |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | 设置时间分段数据的类型。 |
| [setUid(int value)](#setUid-int-) | 设置时间分段数据的唯一标识符 |
| [setUnit(byte value)](#setUnit-byte-) | 设置时间分段数据期间的时间单位。 |
| [setValue(String value)](#setValue-java.lang.String-) | 设置时间分段数据期间每时间单位的值。 |
| [setValueToCost(double value)](#setValueToCost-double-) | `double` 实例，该实例表示此对象的字符串值。 |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


初始化 [TimephasedData](../../com.aspose.tasks/timephaseddata) 类的新实例。

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


创建并初始化用于基于成本的时间分段数据的 [TimephasedData](../../com.aspose.tasks/timephaseddata) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | int | 任务的 UID。 |
| 开始 | java.util.Date | 开始日期时间。 |
| 完成 | java.util.Date | 结束日期时间。 |
| 值 | double | 成本值。 |
| type | 字节 | 时间分段数据类型。 |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


创建并初始化用于基于成本的时间分段数据的 [TimephasedData](../../com.aspose.tasks/timephaseddata) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | int | 任务的 UID。 |
| 开始 | java.util.Date | 开始日期时间。 |
| 完成 | java.util.Date | 结束日期时间。 |
| 值 | double | 成本值。 |
| timeUnit | 字节 | 时间单位类型。 |
| type | 字节 | 时间分段数据类型。 |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


创建并初始化用于材料资源分配的基于单位的时间分段数据的 [TimephasedData](../../com.aspose.tasks/timephaseddata) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | int | 任务的 UID。 |
| 开始 | java.util.Date | 开始日期时间。 |
| 完成 | java.util.Date | 结束日期时间。 |
| 单位 | double | 单位数量。 |
| type | 字节 | 时间分段数据类型。 |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


创建并初始化用于基于工作量的时间分段数据的 [TimephasedData](../../com.aspose.tasks/timephaseddata) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | int | 任务的 UID。 |
| 开始 | java.util.Date | 开始日期时间。 |
| 完成 | java.util.Date | 结束日期时间。 |
| 值 | double | 时间跨度值。 |
| timeUnit | 字节 | 时间单位类型。 |
| type | 字节 | 时间分段数据类型。 |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


获取时间分段数据期间的结束日期。

**Returns:**
java.util.Date - 时间分段数据期间的结束日期。
### getStart() {#getStart--}
```
public final Date getStart()
```


获取时间分段数据期间的开始日期。

**Returns:**
java.util.Date - 时间分段数据期间的开始日期。
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


获取时间分段数据的类型。

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) 属性将在此处指定的类型不适用时被清除。

**Returns:**
byte - 时间分段数据的类型。
### getUid() {#getUid--}
```
public final int getUid()
```


获取时间分段数据的唯一标识符

**Returns:**
int - 时间分段数据的唯一标识符
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


获取时间分段数据期间的时间单位。

**Returns:**
byte - 时间分段数据期间的时间单位。
### getValue() {#getValue--}
```
public final String getValue()
```


获取时间分段数据期间每时间单位的值。

**Returns:**
java.lang.String - 每个时间阶段数据周期的单位时间值。
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


获取 `double` 实例，该实例表示此对象的字符串值。

**Returns:**
double - 对象的浮点表示。
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


获取 double 实例，该实例表示此对象的字符串值。

**Returns:**
double - 对象的时间跨度表示。
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


获取 `double` 实例，该实例表示基于单位的时间分段数据的字符串值。

**Returns:**
double - 此对象的浮点表示。
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


设置时间分段数据期间的结束日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 时间阶段数据周期的结束日期。 |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


设置时间分段数据期间的开始日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 时间阶段数据周期的开始日期。 |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


设置时间分段数据的类型。

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) 属性将在此处指定的类型不适用时被清除。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 字节 | 时间阶段数据的类型。 |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


设置时间分段数据的唯一标识符

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 时间阶段数据的唯一标识符 |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


设置时间分段数据期间的时间单位。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 字节 | 时间阶段数据周期的时间单位。 |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


设置时间分段数据期间每时间单位的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 时间阶段数据周期的单位时间值。 |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


`double` 实例，该实例表示此对象的字符串值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | `double` 实例，该实例表示此对象的字符串值。 |

