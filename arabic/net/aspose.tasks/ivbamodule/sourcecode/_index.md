---
title: "IVbaModule.SourceCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية IVbaModule. تحصل على شفرة المصدر لوحدة VBA"
type: docs
weight: 30
url: /ar/net/aspose.tasks/ivbamodule/sourcecode/
---
## IVbaModule.SourceCode property

يحصل على شفرة المصدر للوحدة VBA

```csharp
public string SourceCode { get; }
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


