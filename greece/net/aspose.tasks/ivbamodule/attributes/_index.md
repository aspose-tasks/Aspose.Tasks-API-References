---
title: "IVbaModule.Attributes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "IVbaModule ιδιότητα. Λαμβάνει μια συλλογή του VbaModuleAttributeCollection"
type: docs
weight: 10
url: /el/net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

Λαμβάνει μια συλλογή του [`VbaModuleAttributeCollection`](../../vbamoduleattributecollection/)

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τα χαρακτηριστικά του μονάδας VBA.

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

### Δείτε επίσης

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


