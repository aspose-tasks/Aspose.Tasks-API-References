---
title: "VbaModule.Attributes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα VbaModule. Λαμβάνει μια συλλογή των χαρακτηριστικών του μονάδας"
type: docs
weight: 30
url: /el/net/aspose.tasks/vbamodule/attributes/
---
## VbaModule.Attributes property

Λαμβάνει μια συλλογή των χαρακτηριστικών της μονάδας.

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
* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


