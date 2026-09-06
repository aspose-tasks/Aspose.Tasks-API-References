---
title: "IVbaModule.Name"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية IVbaModule. تحصل على اسم وحدة VBA"
type: docs
weight: 20
url: /ar/net/aspose.tasks/ivbamodule/name/
---
## IVbaModule.Name property

يحصل على اسم وحدة VBA

```csharp
public string Name { get; }
```

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

* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


