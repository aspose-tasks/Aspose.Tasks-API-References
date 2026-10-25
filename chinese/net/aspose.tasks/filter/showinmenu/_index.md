---
title: "Filter.ShowInMenu"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Filter 属性。获取或设置一个值，指示项目是否在功能区视图选项卡的过滤器下拉列表中显示过滤器名称"
type: docs
weight: 60
url: /zh/net/aspose.tasks/filter/showinmenu/
---
## Filter.ShowInMenu property

获取或设置一个值，指示项目是否在功能区视图选项卡的过滤器下拉列表中显示过滤器名称。

```csharp
public bool ShowInMenu { get; set; }
```

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

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


