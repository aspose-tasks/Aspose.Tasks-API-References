---
title: "VbaModuleCollection.ToList"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة VbaModuleCollection. يحول كائن المجموعة إلى قائمة من كائنات VbaModule"
type: docs
weight: 100
url: /ar/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

يحول كائن المجموعة إلى قائمة من كائنات [`VbaModule`](../../vbamodule/).

```csharp
public List<VbaModule> ToList()
```

### قيمة الإرجاع

قائمة من الكائنات.

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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


