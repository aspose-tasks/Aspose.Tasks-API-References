---
title: "类 Filter"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Filter 类。表示项目中的过滤器"
type: docs
weight: 600
url: /zh/net/aspose.tasks/filter/
---
## Filter class

表示 Project 中的过滤器。

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Filter](filter/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | 获取或设置任务或资源必须满足的条件，以在 MSP 视图中显示。 |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | 获取过滤器的类型。 |
| [Index](../../aspose.tasks/filter/index/) { get; } | 获取 Filters 所包含对象中 `Filter` 对象的索引。 |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | 获取或设置 Filter 对象的名称。 |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | 获取或设置一个值，指示项目是否在功能区视图选项卡的过滤器下拉列表中显示过滤器名称。 |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | 获取或设置一个值，指示是否为该过滤器显示相关的汇总行。 |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | 获取过滤器的唯一标识符。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | 比较此实例与指定的 `Filter` 类实例，并返回它们相对顺序的指示。 |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | 返回一个值，指示此实例是否等于指定的 AssignmentBaseline 对象。 |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | 返回一个值，指示此实例是否等于指定的 AssignmentBaseline 对象。 |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | 返回过滤器的哈希码值。 |
| [operator ==](../../aspose.tasks/filter/op_equality/) | 返回一个值，指示此实例是否等于指定的对象。 |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | 返回一个值，指示此实例是否大于指定的对象。 |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | 返回一个值，指示此实例是否大于或等于指定的对象。 |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | 返回一个值，指示此实例是否不等于指定的对象。 |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | 返回一个值，指示此实例是否小于指定的对象。 |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | 返回一个值，指示此实例是否小于或等于指定的对象。 |

## 示例

展示如何使用过滤器。

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();
Console.WriteLine("Task filters count: " + filters.Count);
foreach (var filter in filters)
{
    Console.WriteLine("Uid: " + filter.Uid);
    Console.WriteLine("Index: " + filter.Index);
    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

// 检查资源过滤器
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


