---
title: "IVbaModule.Name"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "IVbaModule özelliği. VBA modülünün adını alır"
type: docs
weight: 20
url: /tr/net/aspose.tasks/ivbamodule/name/
---
## IVbaModule.Name property

VBA modülünün adını alır

```csharp
public string Name { get; }
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

* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


