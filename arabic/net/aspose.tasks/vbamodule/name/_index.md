---
title: "VbaModule.Name"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية VbaModule. تحصل على اسم وحدة VBA."
type: docs
weight: 40
url: /ar/net/aspose.tasks/vbamodule/name/
---
## VbaModule.Name property

يحصل على اسم وحدة VBA

```csharp
public string Name { get; set; }
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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


