---
title: "الفئة FilterCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.FilterCollection. تحتوي على قائمة من كائنات Filter. تنفّذ واجهة ICollectionFilter."
type: docs
weight: 610
url: /ar/net/aspose.tasks/filtercollection/
---
## FilterCollection class

تحتوي على قائمة من كائنات [`Filter`](../filter/) . تنفّذ واجهة ICollection&lt;Filter&gt;.

```csharp
public class FilterCollection : ICollection<Filter>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/filtercollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks/filtercollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/filtercollection/add/)(Filter) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/filtercollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks/filtercollection/contains/)(Filter) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks/filtercollection/copyto/)(Filter[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetEnumerator](../../aspose.tasks/filtercollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/filtercollection/remove/)(Filter) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |
| [ToList](../../aspose.tasks/filtercollection/tolist/)() | يحوّل مجموعة الفلاتر إلى قائمة من كائنات [`Filter`](../filter/). |

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

* class [Filter](../filter/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


