---
title: "Project.ResourceFilters"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل على جميع تعريفات الفلاتر القائمة على الموارد. ResourceFilters هي مجموعة من كائنات Filter."
type: docs
weight: 760
url: /ar/net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

يحصل على جميع تعريفات الفلاتر القائمة على الموارد. ResourceFilters هي مجموعة من كائنات [`Filter`](../../filter/).

```csharp
public FilterCollection ResourceFilters { get; }
```

## الأمثلة

يعرض كيفية قراءة تعريفات فلاتر المهمة/المورد.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// الوصول إلى فلاتر الموارد
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### انظر أيضًا

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


