---
title: "الفئة Filter"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Filter. تمثل مرشحًا في Project"
type: docs
weight: 600
url: /ar/net/aspose.tasks/filter/
---
## Filter class

يمثل مرشحًا في Project.

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Filter](filter/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | يحصل أو يحدد المعايير التي يجب أن تفي بها المهام أو الموارد لتظهر في عرض MSP. |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | يحصل على نوع المرشح. |
| [Index](../../aspose.tasks/filter/index/) { get; } | يحصل على فهرس كائن `Filter` في الكائن الحاوي للمرشحات. |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | يحصل أو يحدد اسم كائن Filter. |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | يحصل أو يحدد قيمة تشير إلى ما إذا كان المشروع يعرض اسم المرشح في القائمة المنسدلة للمرشح في علامة تبويب View على الشريط. |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كانت صفوف الملخص المرتبطة تُعرض للمرشح. |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | يحصل على المعرف الفريد للمرشح. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | يقارن هذه الحالة بالنسخة المحددة من الفئة `Filter` ويعيد إشارة إلى ترتيبها النسبي. |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية للكيان AssignmentBaseline المحدد. |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية للكيان AssignmentBaseline المحدد. |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | يعيد قيمة رمز تجزئة للمرشح. |
| [operator ==](../../aspose.tasks/filter/op_equality/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أكبر من كائن محدد. |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أكبر من أو مساوية لكائن محدد. |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة غير مساوية لكائن محدد. |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أصغر من كائن محدد. |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أصغر من أو مساوية لكائن محدد. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


