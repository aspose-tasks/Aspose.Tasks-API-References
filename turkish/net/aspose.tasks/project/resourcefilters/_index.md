---
title: "Project.ResourceFilters"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Tüm kaynak tabanlı filtre tanımlarını alır. ResourceFilters, Filter nesnelerinden oluşan bir koleksiyondur."
type: docs
weight: 760
url: /tr/net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

Tüm kaynak tabanlı filtre tanımlarını alır. ResourceFilters, [`Filter`](../../filter/) nesnelerinden oluşan bir koleksiyondur.

```csharp
public FilterCollection ResourceFilters { get; }
```

## Örnekler

Görev/kaynak filtre tanımlarını okumanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// Kaynak filtrelerine eriş
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### Ayrıca Bakınız

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


