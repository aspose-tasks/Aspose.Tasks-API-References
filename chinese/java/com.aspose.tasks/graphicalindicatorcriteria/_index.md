---
title: "GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示与扩展属性关联的一个图形指示器条件。"
type: docs
weight: 115
url: /zh/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

表示与扩展属性关联的一个图形指示器条件。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | 初始化一个新的 [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) 类型实例。 |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | 初始化一个新的 [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) 类型实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | 获取当字段满足条件时要显示的图像索引。 |
| [getRowType()](#getRowType--) | 获取 [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 枚举的值，该枚举指示指示器适用于哪些行。 |
| [getTest()](#getTest--) | 获取在扩展属性值与用于图形指示器应用的准则值之间进行的比较类型。 |
| [getValue1()](#getValue1--) | 获取用于测试扩展属性值的值。 |
| [getValue2()](#getValue2--) | 在比较类型为 'IsWithin' 和 'IsNotWithin' 的情况下，获取用于测试扩展属性值的第二个值。 |
| [toString()](#toString--) | 返回 [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) 类实例的字符串表示。 |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


初始化一个新的 [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) 类型实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowType | int | [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 枚举的值，指示指示器适用于哪些行。 |
| test | int | [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) 的值，表示准则执行的比较类型。 |
| imageIndex | int | 当字段满足条件时要显示的图像索引 |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | 条件检查中使用的值。 |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | 在 'IsWithin' 和 'IsNotWithing' 条件下，条件检查中使用的第二个值（区间结束）。 |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


初始化一个新的 [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) 类型实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowType | int | [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 枚举的值，指示指示器适用于哪些行。 |
| test | int | [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) 的值，表示准则执行的比较类型。 |
| imageIndex | int | 当字段满足条件时要显示的图像索引 |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | 条件检查中使用的值。 |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


获取当字段满足条件时要显示的图像索引。

**Returns:**
int - 当字段满足条件时要显示的图像索引。
### getRowType() {#getRowType--}
```
public final int getRowType()
```


获取 [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 枚举的值，该枚举指示指示器适用于哪些行。

**Returns:**
int - [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 枚举的值，指示指示器适用于哪些行。
### getTest() {#getTest--}
```
public final int getTest()
```


获取在扩展属性值与用于图形指示器应用的准则值之间进行的比较类型。[FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - 在扩展属性值与用于图形指示器应用的准则值之间进行的比较类型。
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


获取用于测试扩展属性值的值。

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


在比较类型为 'IsWithin' 和 'IsNotWithin' 的情况下，获取用于测试扩展属性值的第二个值。

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


返回 [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) 类实例的字符串表示。

**Returns:**
java.lang.String - 此对象的字符串表示。
