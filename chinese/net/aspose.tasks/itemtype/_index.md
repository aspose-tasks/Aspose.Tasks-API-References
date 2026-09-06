---
title: "枚举 ItemType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ItemType 枚举。指定项目的类型。"
type: docs
weight: 920
url: /zh/net/aspose.tasks/itemtype/
---
## ItemType enumeration

指定项目的类型。

```csharp
public enum ItemType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| TaskItem | `0` | 任务项。 |
| ResourceItem | `1` | 资源项。 |
| OtherItem | `2` | 其他项。 |

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


