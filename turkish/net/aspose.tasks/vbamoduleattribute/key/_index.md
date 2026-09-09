---
title: "VbaModuleAttribute.Key"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaModuleAttribute özelliği. VBA modül özniteliğinin anahtarını alır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/vbamoduleattribute/key/
---
## VbaModuleAttribute.Key property

VBA modül özelliğinin anahtarını alır.

```csharp
public string Key { get; }
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


