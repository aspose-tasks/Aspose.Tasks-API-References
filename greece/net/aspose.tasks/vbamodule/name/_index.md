---
title: "VbaModule.Name"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα VbaModule. Λαμβάνει ένα όνομα της μονάδας VBA"
type: docs
weight: 40
url: /el/net/aspose.tasks/vbamodule/name/
---
## VbaModule.Name property

Λαμβάνει ένα όνομα της μονάδας VBA

```csharp
public string Name { get; set; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις μονάδες του έργου VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### Δείτε επίσης

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


