---
title: Class FilterCriteria
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.FilterCriteria 班级. 定义任务或资源必须满足才能显示在 MSP 视图中的条件
type: docs
weight: 630
url: /zh/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

定义任务或资源必须满足才能显示在 MSP 视图中的条件。

```csharp
public class FilterCriteria
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | 获取孩子列表`FilterCriteria`rows. 如果筛选器包含多个条件行，则 And 运算符的作用是必须满足两行的条件才能显示作为此筛选器结果的任务或资源。 Or 的作用运算符是必须满足一行或另一行的条件。 |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | 获取或设置一个[`Field`](./field/)改变. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | 获取或设置与 FieldName、Test 和 Value 建立的条件与过滤器中的其他条件相关。 |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | 获取或设置 FieldName 和 Value 之间的比较类型，作为过滤器的选择标准。 [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | 获取要与 FieldName 指定的字段值进行比较的对象值。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | 返回实例的字符串表示形式`FilterCriteria`类. |

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks/)
* 部件 [Aspose.Tasks](../../)


