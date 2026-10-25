---
title: "Project.ResourceFilters"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Возвращает все определения фильтров, основанных на ресурсах. ResourceFilters представляет собой коллекцию объектов Filter."
type: docs
weight: 760
url: /ru/net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

Возвращает все определения фильтров, основанных на ресурсах. ResourceFilters представляет собой коллекцию объектов [`Filter`](../../filter/).

```csharp
public FilterCollection ResourceFilters { get; }
```

## Примеры

Показывает, как читать определения фильтров задач/ресурсов.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// Доступ к фильтрам ресурсов
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### См. также

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


