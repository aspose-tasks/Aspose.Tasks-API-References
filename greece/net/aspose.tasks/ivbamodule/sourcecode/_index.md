---
title: "IVbaModule.SourceCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "IVbaModule ιδιότητα. Λαμβάνει τον πηγαίο κώδικα του VBA module"
type: docs
weight: 30
url: /el/net/aspose.tasks/ivbamodule/sourcecode/
---
## IVbaModule.SourceCode property

Λαμβάνει τον πηγαίο κώδικα της μονάδας VBA

```csharp
public string SourceCode { get; }
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


