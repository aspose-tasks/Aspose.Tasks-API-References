---
title: "الفئة VbaModule"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.VbaModule. تمثّل وحدة VBA"
type: docs
weight: 2810
url: /ar/net/aspose.tasks/vbamodule/
---
## VbaModule class

يمثّل وحدة VBA.

```csharp
public sealed class VbaModule
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | يحصل على مجموعة من سمات الوحدة. |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | يحصل على اسم وحدة VBA |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | يحصل أو يعيّن شفرة المصدر لوحدة VBA |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | يحصل على نوع الوحدة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | ينشئ مثيلًا من `VbaModule` بنوع VbaModuleType.ClassModule. |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | ينشئ مثيلًا من `VbaModule` بنوع VbaModuleType.ProceduralModule. |

## الأمثلة

يوضح كيفية قراءة وحدات مشروع VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


