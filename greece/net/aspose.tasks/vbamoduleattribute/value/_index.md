---
title: "VbaModuleAttribute.Value"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα VbaModuleAttribute. Λαμβάνει την τιμή του χαρακτηριστικού μονάδας VBA."
type: docs
weight: 20
url: /el/net/aspose.tasks/vbamoduleattribute/value/
---
## VbaModuleAttribute.Value property

Αποκτά την τιμή του χαρακτηριστικού μονάδας VBA.

```csharp
public string Value { get; }
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


