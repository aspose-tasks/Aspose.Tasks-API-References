---
title: "IVbaModule.SourceCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "IVbaModule özelliği. VBA modülünün kaynak kodunu alır"
type: docs
weight: 30
url: /tr/net/aspose.tasks/ivbamodule/sourcecode/
---
## IVbaModule.SourceCode property

VBA modülünün kaynak kodunu alır

```csharp
public string SourceCode { get; }
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


