---
title: "VbaReference.Name"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα VbaReference. Λαμβάνει ή ορίζει το όνομα της αναφοράς VBA"
type: docs
weight: 30
url: /el/net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

Λαμβάνει ή ορίζει το όνομα της αναφοράς VBA.

```csharp
public string Name { get; set; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε αναφορές VBA.

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

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


