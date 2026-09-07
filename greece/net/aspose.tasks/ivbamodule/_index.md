---
title: "Διεπαφή IVbaModule"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Διεπαφή Aspose.Tasks.IVbaModule. Αντιπροσωπεύει μια μονάδα με κώδικα VBA"
type: docs
weight: 880
url: /el/net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

Αντιπροσωπεύει μια μονάδα με κώδικα VBA.

```csharp
public interface IVbaModule
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | Λαμβάνει μια συλλογή του [`VbaModuleAttributeCollection`](../vbamoduleattributecollection/) |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | Λαμβάνει ένα όνομα της μονάδας VBA |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | Λαμβάνει τον πηγαίο κώδικα της μονάδας VBA |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


