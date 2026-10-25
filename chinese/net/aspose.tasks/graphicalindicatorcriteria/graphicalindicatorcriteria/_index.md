---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GraphicalIndicatorCriteria 构造函数。初始化 GraphicalIndicatorCriteria 类型的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

初始化 [`GraphicalIndicatorCriteria`](../) 类型的新实例。

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) 枚举的值，表示指示器适用于哪些行 |
| test | FilterComparisonType | [`FilterComparisonType`](../../filtercomparisontype/) 的值，表示标准执行的比较类型。 |
| imageIndex | Int32 | 字段满足条件时显示的图像索引 |
| value1 | GraphicalIndicatorCriteriaValue | 用于条件检查的值。 |
| value2 | GraphicalIndicatorCriteriaValue | 在 'IsWithin' 和 'IsNotWithing' 条件下用于条件检查的第二个值（区间结束）。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | 当向构造函数传递不正确的参数组合时抛出。 |

### 另见

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

初始化 [`GraphicalIndicatorCriteria`](../) 类型的新实例。

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) 枚举的值，表示指示器适用于哪些行 |
| test | FilterComparisonType | [`FilterComparisonType`](../../filtercomparisontype/) 的值，表示标准执行的比较类型。 |
| imageIndex | Int32 | 字段满足条件时显示的图像索引 |
| value | GraphicalIndicatorCriteriaValue | 用于条件检查的值。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentException | 当向构造函数传递不正确的参数组合时抛出。 |
| ArgumentException | 当 IsWithin 或 IsNotWithing 的值被传递给测试参数时。 |

### 另见

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


