---
title: "IVbaModule.Attributes"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "IVbaModule özelliği. VbaModuleAttributeCollection koleksiyonunu alır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

[`VbaModuleAttributeCollection`](../../vbamoduleattributecollection/) koleksiyonunu alır.

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
* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


