---
title: "Filter"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示 Project 中的筛选器。"
type: docs
weight: 91
url: /zh/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

表示 Project 中的筛选器。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Filter()](#Filter--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | 比较此实例与 [Filter](../../com.aspose.tasks/filter) 类的指定实例，并返回它们相对顺序的指示。 |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | 返回一个值，指示此实例是否等于指定的 AssignmentBaseline 对象。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的 AssignmentBaseline 对象。 |
| [getCriteria()](#getCriteria--) | 获取任务或资源必须满足的条件，以在 MSP 视图中显示。 |
| [getFilterType()](#getFilterType--) | 获取过滤器的类型。 |
| [getIndex()](#getIndex--) | 获取包含对象中 [Filter](../../com.aspose.tasks/filter) 对象的索引。 |
| [getName()](#getName--) | 获取 Filter 对象的名称。 |
| [getShowInMenu()](#getShowInMenu--) | 获取一个值，指示项目是否在功能区的 View 选项卡的 Filter 下拉列表中显示过滤器名称。 |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | 获取一个值，指示是否为该过滤器显示相关的汇总行。 |
| [getUid()](#getUid--) | 获取过滤器的唯一标识符。 |
| [hashCode()](#hashCode--) | 返回过滤器的哈希码值。 |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | 返回一个值，指示此实例是否大于指定的对象。 |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | 返回一个值，指示此实例是否大于或等于指定的对象。 |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | 返回一个值，指示此实例是否不等于指定的对象。 |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | 返回一个值，指示此实例是否小于指定的对象。 |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | 返回一个值，指示此实例是否小于或等于指定的对象。 |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | 设置任务或资源必须满足的条件，以便在 MSP 视图中显示。 |
| [setFilterType(int value)](#setFilterType-int-) | 过滤器的类型。 |
| [setName(String value)](#setName-java.lang.String-) | 设置 Filter 对象的名称。 |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | 设置一个值，指示项目是否在功能区的 View 选项卡的 Filter 下拉列表中显示过滤器名称。 |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | 设置一个值，指示是否为该过滤器显示相关的汇总行。 |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


比较此实例与 [Filter](../../com.aspose.tasks/filter) 类的指定实例，并返回它们相对顺序的指示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | 要与此对象比较的指定 [Filter](../../com.aspose.tasks/filter) 类实例。 |

**Returns:**
int - 表示它们相对顺序的指示。
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


返回一个值，指示此实例是否等于指定的 AssignmentBaseline 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | 要与此实例比较的指定 AssignmentBaseline 对象。 |

**Returns:**
boolean - 如果此实例等于指定的 AssignmentBaseline 对象则返回 true；否则返回 false。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


返回一个值，指示此实例是否等于指定的 AssignmentBaseline 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 要与此实例比较的指定 AssignmentBaseline 对象。 |

**Returns:**
boolean - 如果此实例等于指定的 AssignmentBaseline 对象则返回 true；否则返回 false。
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


获取任务或资源必须满足的条件，以在 MSP 视图中显示。

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


获取过滤器的类型。

**Returns:**
int - 过滤器的类型。
### getIndex() {#getIndex--}
```
public final int getIndex()
```


获取包含对象中 [Filter](../../com.aspose.tasks/filter) 对象的索引。

**Returns:**
int - 包含对象中 [Filter](../../com.aspose.tasks/filter) 对象的索引。
### getName() {#getName--}
```
public final String getName()
```


获取 Filter 对象的名称。

**Returns:**
java.lang.String - Filter 对象的名称。
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


获取一个值，指示项目是否在功能区的 View 选项卡的 Filter 下拉列表中显示过滤器名称。

**Returns:**
boolean - 一个值，指示项目是否在功能区“视图”选项卡的“Filter”下拉列表中显示筛选器名称。
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


获取一个值，指示是否为该过滤器显示相关的汇总行。

**Returns:**
boolean - 一个值，指示是否为该筛选器显示相关的汇总行。
### getUid() {#getUid--}
```
public final int getUid()
```


获取过滤器的唯一标识符。

**Returns:**
int - 筛选器的唯一标识符。
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回过滤器的哈希码值。

**Returns:**
int - 返回此对象的哈希码值。
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 第一个筛选器。 |
| b | [Filter](../../com.aspose.tasks/filter) | 第二个筛选器。 |

**Returns:**
boolean - 一个值，指示此实例是否等于指定的对象
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


返回一个值，指示此实例是否大于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 第一个筛选器。 |
| b | [Filter](../../com.aspose.tasks/filter) | 第二个筛选器。 |

**Returns:**
boolean - 一个值，指示此实例是否大于指定的对象
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


返回一个值，指示此实例是否大于或等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 第一个筛选器。 |
| b | [Filter](../../com.aspose.tasks/filter) | 第二个筛选器。 |

**Returns:**
boolean - 一个值，指示此实例是否大于或等于指定的对象
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


返回一个值，指示此实例是否不等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 第一个筛选器。 |
| b | [Filter](../../com.aspose.tasks/filter) | 第二个筛选器。 |

**Returns:**
boolean - 一个值，指示此实例是否不等于指定的对象
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


返回一个值，指示此实例是否小于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 第一个筛选器。 |
| b | [Filter](../../com.aspose.tasks/filter) | 第二个筛选器。 |

**Returns:**
boolean - 一个值，指示此实例是否小于指定的对象
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


返回一个值，指示此实例是否小于或等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 第一个筛选器。 |
| b | [Filter](../../com.aspose.tasks/filter) | 第二个筛选器。 |

**Returns:**
boolean - 一个值，指示此实例是否小于或等于指定的对象
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


设置任务或资源必须满足的条件，以便在 MSP 视图中显示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | 任务或资源必须满足的条件，以在 MSP 视图中显示。 |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


过滤器的类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 筛选器的类型。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


设置 Filter 对象的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | Filter 对象的名称。 |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


设置一个值，指示项目是否在功能区的 View 选项卡的 Filter 下拉列表中显示过滤器名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示项目是否在功能区“视图”选项卡的“Filter”下拉列表中显示筛选器名称。 |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


设置一个值，指示是否为该过滤器显示相关的汇总行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示是否为该筛选器显示相关的汇总行。 |

