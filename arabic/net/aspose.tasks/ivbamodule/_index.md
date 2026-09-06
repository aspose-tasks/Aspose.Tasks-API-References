---
title: "الواجهة IVbaModule"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الواجهة Aspose.Tasks.IVbaModule. تمثل وحدة تحتوي على كود VBA"
type: docs
weight: 880
url: /ar/net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

تمثل وحدة تحتوي على كود VBA.

```csharp
public interface IVbaModule
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | يحصل على مجموعة من [`VbaModuleAttributeCollection`](../vbamoduleattributecollection/) |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | يحصل على اسم وحدة VBA |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | يحصل على شفرة المصدر للوحدة VBA |

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


