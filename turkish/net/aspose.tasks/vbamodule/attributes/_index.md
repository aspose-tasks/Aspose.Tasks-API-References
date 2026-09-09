---
title: "VbaModule.Attributes"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaModule özelliği. Modülün özniteliklerinin bir koleksiyonunu alır."
type: docs
weight: 30
url: /tr/net/aspose.tasks/vbamodule/attributes/
---
## VbaModule.Attributes property

Modülün özniteliklerinin bir koleksiyonunu alır.

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## Örnekler

VBA modülünün özniteliklerini nasıl okuyacağını gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("VB Name: " + attribute.Key);
        Console.WriteLine("Module: " + attribute.Value);
    }
}
```

### Ayrıca Bakınız

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


