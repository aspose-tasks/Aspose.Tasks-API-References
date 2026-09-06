---
title: "类 FilterCriteria"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.FilterCriteria 类。定义任务或资源必须满足的条件，以在 MSP 视图中显示"
type: docs
weight: 630
url: /zh/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

定义任务或资源必须满足的条件，以在 MSP 视图中显示。

```csharp
public class FilterCriteria
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | 获取子 `FilterCriteria` 行的列表。如果过滤器包含多个条件行，则 And 运算符的效果是必须同时满足两行的条件，任务或资源才会作为此过滤器的结果显示。Or 运算符的效果是只需满足其中一行的条件即可。 |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | 获取或设置一个要更改的 [`Field`](./field/)。 |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | 获取或设置使用 FieldName、Test 和 Value 建立的标准，该标准与过滤器中的其他标准相关。 |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | 获取或设置在 FieldName 与 Value 之间进行的比较类型，该比较用作过滤器的选择标准。[`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | 获取用于与 FieldName 指定的字段值进行比较的对象值。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | 获取 FilterCriteria 的右侧值是否为字段引用，而非常量值。 |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | 设置其值将与 FieldName 指定的字段值进行比较的字段。 |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | 返回 `FilterCriteria` 类实例的字符串表示。 |

## 示例

展示如何读取任务过滤条件。

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// 将过滤条件打印为字符串
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


