---
title: "VbaProject.References"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα VbaProject. Λαμβάνει μια συλλογή του VbaReferenceCollection"
type: docs
weight: 70
url: /el/net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

Λαμβάνει μια συλλογή του [`VbaReferenceCollection`](../../vbareferencecollection/)

```csharp
public VbaReferenceCollection References { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε πληροφορίες αναφοράς έργου VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Δείτε επίσης

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


