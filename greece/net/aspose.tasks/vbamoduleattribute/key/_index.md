---
title: "VbaModuleAttribute.Key"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα VbaModuleAttribute. Λαμβάνει το κλειδί της ιδιότητας μονάδας VBA"
type: docs
weight: 10
url: /el/net/aspose.tasks/vbamoduleattribute/key/
---
## VbaModuleAttribute.Key property

Αποκτά το κλειδί του χαρακτηριστικού μονάδας VBA.

```csharp
public string Key { get; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τις ιδιότητες της μονάδας VBA.

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

### Δείτε επίσης

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


