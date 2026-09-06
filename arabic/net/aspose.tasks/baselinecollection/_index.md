---
title: "الفئة BaselineCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.BaselineCollection. تمثل مجموعة من كائنات Baseline."
type: docs
weight: 120
url: /ar/net/aspose.tasks/baselinecollection/
---
## BaselineCollection class

تمثل مجموعة من كائنات [`Baseline`](../baseline/).

```csharp
public class BaselineCollection : IList<Baseline>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/baselinecollection/count/) { get; } | يحصل على عدد الكائنات الموجودة في كائن BaselineCollection هذا. |
| [Item](../../aspose.tasks/baselinecollection/item/) { get; set; } | يرجع العنصر عند الفهرس المحدد. |
| [ParentResource](../../aspose.tasks/baselinecollection/parentresource/) { get; } | يحصل على العنصر الأب [`Resource`](../resource/) لهذه المجموعة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/baselinecollection/add/)(Baseline) | هذا هو تنفيذ النموذج الأولي لطريقة Add في ICollection، والذي يرمي فقط NotSupportedException |
| [GetEnumerator](../../aspose.tasks/baselinecollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/baselinecollection/remove/)(Baseline) | يزيل الخط الأساسي من هذه المجموعة. |
| [ToList](../../aspose.tasks/baselinecollection/tolist/)() | تحويل كائن BaselineCollection إلى قائمة من كائنات [`Baseline`](../baseline/). |

## الأمثلة

يوضح كيفية العمل مع مجموعات Baseline.

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// قراءة معلومات الخط الأساسي
foreach (var baseline in resource.Baselines)
{
    Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
    Console.WriteLine("Cost: " + baseline.Cost);
    Console.WriteLine("Work: " + baseline.Work);
    Console.WriteLine("BCWP: " + baseline.Bcwp);
    Console.WriteLine("BCWS: " + baseline.Bcws);
    Console.WriteLine();
}

Console.WriteLine("Delete all baselines: ");
List<Baseline> baselines = resource.Baselines.ToList();
foreach (var baseline in baselines)
{
    Console.WriteLine("Delete baseline with name: " + baseline.BaselineNumber);
    resource.Baselines.Remove(baseline);
}
```

### انظر أيضًا

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


