---
title: "Project.ResourceFilters"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取所有基于资源的过滤器定义。ResourceFilters 是 Filter 对象的集合。"
type: docs
weight: 760
url: /zh/net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

获取所有基于资源的过滤器定义。ResourceFilters 是一个 [`Filter`](../../filter/) 对象的集合。

```csharp
public FilterCollection ResourceFilters { get; }
```

## 示例

展示如何读取任务/资源过滤器定义。

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// 访问资源过滤器
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### 另见

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


