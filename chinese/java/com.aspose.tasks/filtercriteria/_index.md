---
title: "FilterCriteria"
second_title: "Aspose.Tasks for Java API 参考"
description: "定义任务或资源必须满足的条件，以在 MSP 视图中显示。"
type: docs
weight: 94
url: /zh/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

定义任务或资源必须满足的条件，以在 MSP 视图中显示。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | 获取子 [FilterCriteria](../../com.aspose.tasks/filtercriteria) 行的列表。 |
| [getField()](#getField--) | 获取一个 `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) 进行更改。 |
| [getOperation()](#getOperation--) | 获取使用 FieldName、Test 和 Value 建立的标准，该标准与过滤器中的其他标准相关。 |
| [getTest()](#getTest--) | 获取在 FieldName 与 Value 之间进行的比较类型，该类型作为过滤器的选择标准。 |
| [getValues()](#getValues--) | 获取用于与由 FieldName 指定的字段值进行比较的对象值。 |
| [isValueAField()](#isValueAField--) | 获取 FilterCriteria 的右侧值是否为字段引用，而非常量值。 |
| [isValueAField(int index)](#isValueAField-int-) | 获取 FilterCriteria 索引处的值是否为字段引用，而非常量值。 |
| [setField(int value)](#setField-int-) | 设置一个 `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) 进行更改。 |
| [setOperation(int value)](#setOperation-int-) | 设置使用 FieldName、Test 和 Value 建立的准则，使其与过滤器中的其他准则相关。 |
| [setTest(int value)](#setTest-int-) | 设置 FieldName 与 Value 之间的比较类型，该比较类型作为过滤器的选择准则。 |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | 设置索引处的对象值，以与 FieldName 指定的字段值进行比较。 |
| [setValue(Object value)](#setValue-java.lang.Object-) | 设置对象值，以与 FieldName 指定的字段值进行比较。 |
| [setValueByField(int value)](#setValueByField-int-) | 设置字段，其值将与 FieldName 指定的字段值进行比较。 |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | 设置索引处的字段，其值将与 FieldName 指定的字段值进行比较。 |
| [toString()](#toString--) | 返回 [FilterCriteria](../../com.aspose.tasks/filtercriteria) 类实例的字符串表示形式。 |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


获取子 [FilterCriteria](../../com.aspose.tasks/filtercriteria) 行的列表。如果过滤器包含多个准则行，则 And 运算符的效果是必须同时满足两行的准则，任务或资源才会作为此过滤器的结果显示。Or 运算符的效果是只需满足其中一行的准则即可。

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - 子 [FilterCriteria](../../com.aspose.tasks/filtercriteria) 行的列表。
### getField() {#getField--}
```
public final int getField()
```


获取一个 `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) 进行更改。

**Returns:**
int - 要更改的 `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-))。
### getOperation() {#getOperation--}
```
public final int getOperation()
```


获取使用 FieldName、Test 和 Value 建立的标准，该标准与过滤器中的其他标准相关。

**Returns:**
int - 使用 FieldName、Test 和 Value 建立的准则，与过滤器中的其他准则相关。
### getTest() {#getTest--}
```
public final int getTest()
```


获取 FieldName 与 Value 之间的比较类型，该类型作为过滤器的选择准则。[FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - FieldName 与 Value 之间的比较类型，作为过滤器的选择准则。
### getValues() {#getValues--}
```
public final Object[] getValues()
```


获取用于与由 FieldName 指定的字段值进行比较的对象值。

**Returns:**
java.lang.Object[] - 用于与 FieldName 指定的字段值进行比较的对象值。
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


获取 FilterCriteria 的右侧值是否为字段引用，而非常量值。

**Returns:**
boolean - 表示 FilterCriteria 的右侧值是否为字段引用，而非常量值。
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


获取 FilterCriteria 索引处的值是否为字段引用，而非常量值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 值的索引 |

**Returns:**
boolean - 表示 FilterCriteria 索引处的右侧值是否为字段引用，而非常量值。
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


设置一个 `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) 进行更改。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | int | 一个 `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) 用于更改。 |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


设置使用 FieldName、Test 和 Value 建立的准则，使其与过滤器中的其他准则相关。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 使用 FieldName、Test 和 Value 建立的准则，与过滤器中的其他准则相关。 |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


设置 FieldName 与 Value 之间的比较类型，该类型作为过滤器的选择准则。[FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | FieldName 与 Value 之间的比较类型，作为过滤器的选择准则。 |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


设置索引处的对象值，以与 FieldName 指定的字段值进行比较。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 值的索引。 |
| 值 | java.lang.Object | 对象值，将作为过滤准则索引处的右侧值。 |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


设置对象值，以与 FieldName 指定的字段值进行比较。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object | 对象值，将作为过滤准则的右侧值。 |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


设置字段，其值将与 FieldName 指定的字段值进行比较。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 字段，将作为过滤准则的右侧值。 |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


设置索引处的字段，其值将与 FieldName 指定的字段值进行比较。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 值的索引 |
| 值 | int | 字段将在过滤条件的索引处用作右侧值。 |

### toString() {#toString--}
```
public String toString()
```


返回 [FilterCriteria](../../com.aspose.tasks/filtercriteria) 类实例的字符串表示形式。

**Returns:**
java.lang.String - 此对象的字符串表示。
