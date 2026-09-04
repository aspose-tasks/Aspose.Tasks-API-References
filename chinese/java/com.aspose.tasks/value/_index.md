---
title: "值"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示值列表中的一个值。"
type: docs
weight: 333
url: /zh/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

表示值列表中的一个值。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Value()](#Value--) | 初始化一个新的 [Value](../../com.aspose/tasks/value) 类的实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDateValue()](#getDateValue--) | 获取实际值（如果可以表示为 DateTime）。 |
| [getDescription()](#getDescription--) | 获取值的描述。 |
| [getDuration()](#getDuration--) | 获取用于表示 Duration 的实际值。 |
| [getId()](#getId--) | 获取跨项目的值的唯一标识符。 |
| [getNumericValue()](#getNumericValue--) | 获取用于表示数字或成本值的实际值。 |
| [getPhonetic()](#getPhonetic--) | 获取关于自定义字段名称的拼音信息。 |
| [getStringValue()](#getStringValue--) | 获取用于表示文本字符串的实际值。 |
| [getVal()](#getVal--) | 获取内部表示中的实际值。 |
| [getValueGuid()](#getValueGuid--) | 获取在整个项目中标识此值的 GUID。 |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | 设置实际值（如果可以表示为 DateTime）。 |
| [setDescription(String value)](#setDescription-java.lang.String-) | 设置值的描述。 |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | 设置用于表示 Duration 的实际值。 |
| [setId(int value)](#setId-int-) | 设置跨项目的值的唯一标识符。 |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | 设置用于表示数字或成本值的实际值。 |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | 设置关于自定义字段名称的拼音信息。 |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | 设置用于表示文本字符串的实际值。 |
| [setVal(String value)](#setVal-java.lang.String-) | 设置内部表示中的实际值。 |
### Value() {#Value--}
```
public Value()
```


初始化一个新的 [Value](../../com.aspose/tasks/value) 类的实例。

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


获取实际值（如果可以表示为 DateTime）。默认值为 DateTime\#MinValue.MinValue。

--------------------

在需要设置 DateTime 值时，优先使用此属性而不是 `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))。

**Returns:**
java.util.Date - 如果可以表示为 DateTime，则为实际值。
### getDescription() {#getDescription--}
```
public final String getDescription()
```


获取值的描述。

**Returns:**
java.lang.String - 值的描述。
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


获取用于表示 Duration 的实际值。

--------------------

在需要设置 Duration 值时，优先使用此属性而不是 `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


获取跨项目的值的唯一标识符。

对于不同的 [Value](../../com.aspose.tasks/value) 实例，避免使用相同的标识符很重要。

最小的 `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) 值为 `1`。

**Returns:**
int - 项目中值的唯一标识符。
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


获取用于表示数字或成本值的实际值。

--------------------

在需要设置 Number 或 Cost 值时，优先使用此属性而不是 `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))。

**Returns:**
java.math.BigDecimal - 用于表示数字或成本值的实际值。
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


获取关于自定义字段名称的拼音信息。

**Returns:**
java.lang.String - 自定义字段名称的拼音信息。
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


获取用于表示文本字符串的实际值。

--------------------

在需要设置 Text 值时，优先使用此属性而不是 `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))。

**Returns:**
java.lang.String - 用于表示 Text 字符串的实际值。
### getVal() {#getVal--}
```
public final String getVal()
```


获取内部表示中的实际值。建议使用下面列出的强类型属性。

--------------------

如果要设置 Text 值，建议使用强类型的 `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) 属性。

如果要设置 Number 或 Cost 值，建议使用强类型的 `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) 属性。

如果要设置 Date/Start/Finish 值，建议使用强类型的 `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) 属性。

如果要设置 Duration 值，建议使用强类型的 `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) 属性。

如果您的类型未列出，请使用 `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) 属性。

**Returns:**
java.lang.String - 内部表示中的实际值。
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


获取在整个项目中标识此值的 GUID。

**Returns:**
java.util.UUID - 在整个项目中标识此值的 GUID。
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


如果可以表示为 DateTime，则设置实际值。默认值为 DateTime\#MinValue.MinValue。

--------------------

在需要设置 DateTime 值时，优先使用此属性而不是 `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 如果可以表示为 DateTime，则为实际值。 |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


设置值的描述。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 值的描述。 |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


设置用于表示 Duration 的实际值。

--------------------

在需要设置 Duration 值时，优先使用此属性而不是 `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 用于表示 Duration 的实际值。 |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


设置跨项目的值的唯一标识符。

对于不同的 [Value](../../com.aspose.tasks/value) 实例，避免使用相同的标识符很重要。

最小的 `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) 值为 `1`。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 跨项目的值的唯一标识符。 |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


设置用于表示数字或成本值的实际值。

--------------------

在需要设置 Number 或 Cost 值时，优先使用此属性而不是 `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | 用于表示数字或费用值的实际值。 |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


设置关于自定义字段名称的拼音信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 关于自定义字段名称的拼音信息。 |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


设置用于表示文本字符串的实际值。

--------------------

在需要设置 Text 值时，优先使用此属性而不是 `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 用于表示文本字符串的实际值。 |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


设置内部表示中的实际值。建议使用下面列出的强类型属性。

--------------------

如果要设置 Text 值，建议使用强类型的 `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) 属性。

如果要设置 Number 或 Cost 值，建议使用强类型的 `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) 属性。

如果您想设置 Date/Start/Finish 值，建议使用强类型的 `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) 属性。

如果要设置 Duration 值，建议使用强类型的 `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) 属性。

如果您的类型未列出，请使用 `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) 属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 内部表示中的实际值。 |

