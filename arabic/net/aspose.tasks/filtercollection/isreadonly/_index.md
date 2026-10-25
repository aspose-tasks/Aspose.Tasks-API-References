---
title: "FilterCollection.IsReadOnly"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية FilterCollection. تحصل على قيمة تشير إلى ما إذا كان هذا التجميع للقراءة فقط، وإلا false"
type: docs
weight: 20
url: /ar/net/aspose.tasks/filtercollection/isreadonly/
---
## FilterCollection.IsReadOnly property

يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false.

```csharp
public bool IsReadOnly { get; }
```

## الأمثلة

يظهر كيفية العمل مع مجموعات الفلاتر.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

// التكرار عبر فلاتر المهام
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

// التكرار عبر فلاتر الموارد
Console.WriteLine("Project.ResourceFilters count: " + project.ResourceFilters.Count);
foreach (var filter in project.ResourceFilters)
{
    Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + filter.FilterType);
    Console.WriteLine("Resource filter ShowInMenu" + filter.ShowInMenu);
    Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// مسح فلاتر المشروع الآخر
otherProject.TaskFilters.Clear();

// نسخ الفلاتر إلى مشروع آخر
var filters = new Filter[project.TaskFilters.Count];
project.TaskFilters.CopyTo(filters, 0);

foreach (var filter in filters)
{
    otherProject.TaskFilters.Add(filter);
}

// إضافة فلتر مهمة مخصص
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

// إزالة جميع الفلاتر
List<Filter> filtersToDelete = otherProject.TaskFilters.ToList();
foreach (var filter in filtersToDelete)
{
    otherProject.TaskFilters.Remove(filter);
}
```

### انظر أيضًا

* class [FilterCollection](../)
* namespace [Aspose.Tasks](../../filtercollection/)
* assembly [Aspose.Tasks](../../../)


