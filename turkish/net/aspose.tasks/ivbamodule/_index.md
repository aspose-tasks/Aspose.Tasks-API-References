---
title: "Arayüz IVbaModule"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.IVbaModule arayüzü. VBA kodlu bir modülü temsil eder"
type: docs
weight: 880
url: /tr/net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

VBA kodlu bir modülü temsil eder.

```csharp
public interface IVbaModule
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | [`VbaModuleAttributeCollection`](../vbamoduleattributecollection/) koleksiyonunu alır. |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | VBA modülünün adını alır |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | VBA modülünün kaynak kodunu alır |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


