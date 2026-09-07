---
title: "Project.ResourceFilters"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan semua definisi filter berbasis sumber daya. ResourceFilters adalah koleksi objek Filter."
type: docs
weight: 760
url: /id/net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

Mendapatkan semua definisi filter berbasis sumber daya. ResourceFilters adalah koleksi objek [`Filter`](../../filter/).

```csharp
public FilterCollection ResourceFilters { get; }
```

## Contoh

Menampilkan cara membaca definisi filter tugas/sumber daya.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// Akses filter sumber daya
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### Lihat Juga

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


