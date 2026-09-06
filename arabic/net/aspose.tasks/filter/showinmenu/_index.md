---
title: "Filter.ShowInMenu"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Filter property. يحصل أو يعيّن قيمة تشير إلى ما إذا كان المشروع يعرض اسم الفلتر في قائمة الفلتر المنسدلة في علامة تبويب العرض على الشريط"
type: docs
weight: 60
url: /ar/net/aspose.tasks/filter/showinmenu/
---
## Filter.ShowInMenu property

يحصل أو يحدد قيمة تشير إلى ما إذا كان المشروع يعرض اسم المرشح في القائمة المنسدلة للمرشح في علامة تبويب View على الشريط.

```csharp
public bool ShowInMenu { get; set; }
```

## الأمثلة

يظهر كيفية العمل مع المرشحات.

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

// تحقق من مرشحات الموارد
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### انظر أيضًا

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


