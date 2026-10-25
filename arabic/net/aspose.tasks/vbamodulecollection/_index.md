---
title: "الفئة VbaModuleCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.VbaModuleCollection. تمثّل مجموعة من كائنات VbaModule."
type: docs
weight: 2840
url: /ar/net/aspose.tasks/vbamodulecollection/
---
## VbaModuleCollection class

تمثّل مجموعة من كائنات [`VbaModule`](../vbamodule/).

```csharp
public class VbaModuleCollection : ICollection<VbaModule>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/vbamodulecollection/count/) { get; } |  |
| [IsReadOnly](../../aspose.tasks/vbamodulecollection/isreadonly/) { get; } |  |
| [Item](../../aspose.tasks/vbamodulecollection/item/) { get; } | يحصل على الوحدة في الفهرس المحدد. (2 مؤشرات) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/vbamodulecollection/add/)(VbaModule) |  |
| [Clear](../../aspose.tasks/vbamodulecollection/clear/)() |  |
| [Contains](../../aspose.tasks/vbamodulecollection/contains/)(VbaModule) |  |
| [CopyTo](../../aspose.tasks/vbamodulecollection/copyto/)(VbaModule[], int) |  |
| [GetEnumerator](../../aspose.tasks/vbamodulecollection/getenumerator/)() |  |
| [Remove](../../aspose.tasks/vbamodulecollection/remove/)(VbaModule) |  |
| [ToList](../../aspose.tasks/vbamodulecollection/tolist/)() | يحوّل كائن المجموعة إلى قائمة من كائنات [`VbaModule`](../vbamodule/). |

## الأمثلة

يوضح كيفية التكرار عبر وحدات VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var vbaProject = project.VbaProject;

Console.WriteLine("Total Modules Count: " + vbaProject.Modules.Count);
foreach (VbaModule module in vbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Module Type: " + module.Type);
    Console.WriteLine("Source Code: " + module.SourceCode);
    Console.WriteLine();
}
```

### انظر أيضًا

* class [VbaModule](../vbamodule/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


