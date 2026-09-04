---
title: "GraphicalIndicatorCriteriaValue"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示用于图形指示器条件检查的值。"
type: docs
weight: 117
url: /zh/java/com.aspose.tasks/graphicalindicatorcriteriavalue/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteriaValue
```

表示用于图形指示器条件检查的值。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GraphicalIndicatorCriteriaValue(BigDecimal value)](#GraphicalIndicatorCriteriaValue-java.math.BigDecimal-) | 创建一个 GraphicalIndicatorCriteriaValue 类的实例，使用常量 BigDecimal 值。 |
| [GraphicalIndicatorCriteriaValue(Date dateValue)](#GraphicalIndicatorCriteriaValue-java.util.Date-) | 创建一个 GraphicalIndicatorCriteriaValue 类的实例，使用常量 Date 值。 |
| [GraphicalIndicatorCriteriaValue(String textValue)](#GraphicalIndicatorCriteriaValue-java.lang.String-) | 创建一个 GraphicalIndicatorCriteriaValue 类的实例，使用常量 String 值。 |
| [GraphicalIndicatorCriteriaValue(Duration durationValue)](#GraphicalIndicatorCriteriaValue-com.aspose.tasks.Duration-) | 创建一个 GraphicalIndicatorCriteriaValue 类的实例，使用常量 Duration 值。 |
| [GraphicalIndicatorCriteriaValue(boolean flagValue)](#GraphicalIndicatorCriteriaValue-boolean-) | 创建一个 GraphicalIndicatorCriteriaValue 类的实例，使用常量 flag（boolean）值。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [createFieldLink(int field)](#createFieldLink-int-) | 创建一个 GraphicalIndicatorCriteriaValue 类的实例，表示指定 MS Project 字段的值。 |
| [getRawValue()](#getRawValue--) | 获取 Field 值的底层常量。 |
| [isFieldLink()](#isFieldLink--) | 获取当前实例是否为字段链接（表示字段的值）。 |
| [toString()](#toString--) | 返回表示当前对象的字符串。 |
### GraphicalIndicatorCriteriaValue(BigDecimal value) {#GraphicalIndicatorCriteriaValue-java.math.BigDecimal-}
```
public GraphicalIndicatorCriteriaValue(BigDecimal value)
```


创建一个 GraphicalIndicatorCriteriaValue 类的实例，使用常量 BigDecimal 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.math.BigDecimal | BigDecimal 值 |

### GraphicalIndicatorCriteriaValue(Date dateValue) {#GraphicalIndicatorCriteriaValue-java.util.Date-}
```
public GraphicalIndicatorCriteriaValue(Date dateValue)
```


创建一个 GraphicalIndicatorCriteriaValue 类的实例，使用常量 Date 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dateValue | java.util.Date | Date 值 |

### GraphicalIndicatorCriteriaValue(String textValue) {#GraphicalIndicatorCriteriaValue-java.lang.String-}
```
public GraphicalIndicatorCriteriaValue(String textValue)
```


创建一个 GraphicalIndicatorCriteriaValue 类的实例，使用常量 String 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| textValue | java.lang.String | String 值 |

### GraphicalIndicatorCriteriaValue(Duration durationValue) {#GraphicalIndicatorCriteriaValue-com.aspose.tasks.Duration-}
```
public GraphicalIndicatorCriteriaValue(Duration durationValue)
```


创建一个 GraphicalIndicatorCriteriaValue 类的实例，使用常量 Duration 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| durationValue | [Duration](../../com.aspose.tasks/duration) | Duration 值 |

### GraphicalIndicatorCriteriaValue(boolean flagValue) {#GraphicalIndicatorCriteriaValue-boolean-}
```
public GraphicalIndicatorCriteriaValue(boolean flagValue)
```


创建一个 GraphicalIndicatorCriteriaValue 类的实例，使用常量 flag（boolean）值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| flagValue | boolean | flag（boolean）值 |

### createFieldLink(int field) {#createFieldLink-int-}
```
public static GraphicalIndicatorCriteriaValue createFieldLink(int field)
```


创建一个 GraphicalIndicatorCriteriaValue 类的实例，表示指定 MS Project 字段的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 字段 | int | 指定的字段 |

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - instance of GraphicalIndicatorCriteriaValue class representing the value of the specified field
### getRawValue() {#getRawValue--}
```
public final Object getRawValue()
```


获取 Field 值的底层常量。

**Returns:**
java.lang.Object - Field 值的底层常量
### isFieldLink() {#isFieldLink--}
```
public final boolean isFieldLink()
```


获取当前实例是否为字段链接（表示字段的值）。

**Returns:**
boolean - 当前实例是否为字段链接（表示字段的值）
### toString() {#toString--}
```
public String toString()
```


返回表示当前对象的字符串。

**Returns:**
java.lang.String - 表示当前对象的字符串
