---
title: "IVbaModule.Name"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "IVbaModule ιδιότητα. Λαμβάνει ένα όνομα του VBA module"
type: docs
weight: 20
url: /el/net/aspose.tasks/ivbamodule/name/
---
## IVbaModule.Name property

Λαμβάνει ένα όνομα της μονάδας VBA

```csharp
public string Name { get; }
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

* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


