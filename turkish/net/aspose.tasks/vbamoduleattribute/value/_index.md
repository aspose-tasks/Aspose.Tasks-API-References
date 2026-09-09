---
title: "VbaModuleAttribute.Value"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaModuleAttribute özelliği. VBA modül özniteliğinin değerini alır"
type: docs
weight: 20
url: /tr/net/aspose.tasks/vbamoduleattribute/value/
---
## VbaModuleAttribute.Value property

VBA modül özelliğinin değerini alır.

```csharp
public string Value { get; }
```

## Örnekler

VBA modül öznitelikleriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### Ayrıca Bakınız

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


