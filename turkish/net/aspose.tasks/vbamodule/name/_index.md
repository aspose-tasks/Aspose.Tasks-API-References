---
title: "VbaModule.Name"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaModule özelliği. VBA modülünün adını alır."
type: docs
weight: 40
url: /tr/net/aspose.tasks/vbamodule/name/
---
## VbaModule.Name property

VBA modülünün adını alır

```csharp
public string Name { get; set; }
```

## Örnekler

VBA projesinin modüllerinin nasıl okunacağını gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### Ayrıca Bakınız

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


