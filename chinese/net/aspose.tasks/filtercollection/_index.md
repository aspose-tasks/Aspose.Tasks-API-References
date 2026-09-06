---
title: "类 FilterCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.FilterCollection 类。包含 Filter 对象的列表。实现 ICollectionFilter 接口"
type: docs
weight: 610
url: /zh/net/aspose.tasks/filtercollection/
---
## FilterCollection class

包含一个 [`Filter`](../filter/) 对象列表。实现 ICollection&lt;Filter&gt; 接口。

```csharp
public class FilterCollection : ICollection<Filter>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/filtercollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/filtercollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/filtercollection/add/)(Filter) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/filtercollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/filtercollection/contains/)(Filter) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/filtercollection/copyto/)(Filter[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/filtercollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/filtercollection/remove/)(Filter) | 从此集合中移除特定对象的第一次出现。 |
| [ToList](../../aspose.tasks/filtercollection/tolist/)() | 将过滤器集合转换为 [`Filter`](../filter/) 对象列表。 |

## 示例

展示如何使用过滤器集合。

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

// 遍历任务过滤器
Console.WriteLine("Print task filters of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Filters Count: " + project.TaskFilters.Count);
foreach (var filter in project.TaskFilters)
{
    Console.WriteLine("All Tasks: " + filter.Name);
    Console.WriteLine("Task Item: " + filter.FilterType);
    Console.WriteLine("Task Filters Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Task filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
    Console.WriteLine();
}

// 遍历资源过滤器
Console.WriteLine("Project.ResourceFilters count: " + project.ResourceFilters.Count);
foreach (var filter in project.ResourceFilters)
{
    Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + filter.FilterType);
    Console.WriteLine("Resource filter ShowInMenu" + filter.ShowInMenu);
    Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// 清除其他项目的过滤器
otherProject.TaskFilters.Clear();

// 将过滤器复制到其他项目
var filters = new Filter[project.TaskFilters.Count];
project.TaskFilters.CopyTo(filters, 0);

foreach (var filter in filters)
{
    otherProject.TaskFilters.Add(filter);
}

// 添加自定义任务过滤器
var customFilter = new Filter();
customFilter.Name = "Custom Filter";
customFilter.ShowInMenu = true;
customFilter.ShowRelatedSummaryRows = true;

if (!otherProject.TaskFilters.Contains(customFilter))
{
    if (!otherProject.TaskFilters.IsReadOnly)
    {
        otherProject.TaskFilters.Add(customFilter);
    }
}

// 删除所有过滤器
List<Filter> filtersToDelete = otherProject.TaskFilters.ToList();
foreach (var filter in filtersToDelete)
{
    otherProject.TaskFilters.Remove(filter);
}
```

### 另见

* class [Filter](../filter/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


