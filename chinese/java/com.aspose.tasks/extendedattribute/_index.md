---
title: "ExtendedAttribute"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示扩展属性。"
type: docs
weight: 81
url: /zh/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

表示扩展属性。

--------------------

当前支持从 MSP Xml 2003/2007 和 mpp 2003 读取的所有类型的扩展属性。对于 MSP mpp 2007，支持读取所有扩展属性，除持续时间和标志外。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | 获取属性定义。 |
| [getDateValue()](#getDateValue--) | 获取日期类型属性（Date、Start、Finish）的值。 |
| [getDurationValue()](#getDurationValue--) | 获取 'Duration' 类型属性的值。 |
| [getFieldId()](#getFieldId--) | 获取字段的 ID。 |
| [getFlagValue()](#getFlagValue--) | 获取指示 'Flag' 类型属性是否设置了标志的值。 |
| [getNumericValue()](#getNumericValue--) | 获取数值类型属性（Cost、Number）的值。 |
| [getTextValue()](#getTextValue--) | 获取 'Text' 类型属性的值。 |
| [getValueGuid()](#getValueGuid--) | 获取查找值的 GUID。 |
| [getValueReadOnly()](#getValueReadOnly--) | 获取指示此 [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) 实例的值是否只读的值。 |
| [isErrorValue()](#isErrorValue--) | 获取扩展属性值的计算是否导致错误。 |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | 为日期类型属性（Date、Start、Finish）设置值。 |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | 为具有 'Duration' 类型的属性设置值。 |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | 设置一个值，指示是否为具有 'Flag' 类型的属性设置了标志。 |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | 为具有数值类型 (Cost, Number) 的属性设置值。 |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | 为具有 'Text' 类型的属性设置值。 |
| [toString()](#toString--) | 返回扩展属性的简短字符串表示。 |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


获取属性定义。

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


获取日期类型属性（Date、Start、Finish）的值。

**Returns:**
java.util.Date - 为具有日期类型（Date, Start, Finish）的属性提供的值。
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


获取 'Duration' 类型属性的值。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


获取字段的 ID。

**Returns:**
java.lang.String - 字段的标识符。
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


获取指示 'Flag' 类型属性是否设置了标志的值。

**Returns:**
boolean - 指示是否为具有 'Flag' 类型的属性设置了标志的值。
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


获取数值类型属性（Cost、Number）的值。

**Returns:**
java.math.BigDecimal - 为具有数值类型（Cost, Number）的属性提供的值。
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


获取 'Text' 类型属性的值。

**Returns:**
java.lang.String - 为具有 'Text' 类型的属性提供的值。
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


获取查找值的 GUID。

--------------------

不应直接设置，而应使用 ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) 来创建带有查找值的扩展属性。

**Returns:**
java.lang.String - 查找值的 GUID。
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


获取指示此 [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) 实例的值是否只读的值。

Value: 如果在此对象的 [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) 中定义了公式或汇总，则返回 true。

**Returns:**
boolean - 指示此 [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) 实例的值是否为只读的值。
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


获取扩展属性值的计算是否导致错误。

**Returns:**
boolean - 扩展属性值的计算是否导致错误。
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


为日期类型属性（Date、Start、Finish）设置值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 为具有日期类型（Date, Start, Finish）的属性提供的值。 |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


为具有 'Duration' 类型的属性设置值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 为具有 'Duration' 类型的属性提供的值。 |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


设置一个值，指示是否为具有 'Flag' 类型的属性设置了标志。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否为具有 'Flag' 类型的属性设置了标志的值。 |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


为具有数值类型 (Cost, Number) 的属性设置值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | 为具有数值类型（Cost, Number）的属性提供的值。 |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


为具有 'Text' 类型的属性设置值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 为具有 'Text' 类型的属性提供的值。 |

### toString() {#toString--}
```
public String toString()
```


返回扩展属性的简短字符串表示。

**Returns:**
java.lang.String - 扩展属性的字符串表示。
