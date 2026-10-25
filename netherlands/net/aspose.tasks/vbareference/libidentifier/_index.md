---
title: "VbaReference.LibIdentifier"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaReference-eigenschap. Haalt de identifier van de bibliotheek op"
type: docs
weight: 20
url: /nl/net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

Haalt de identifier van de bibliotheek op.

```csharp
public string LibIdentifier { get; }
```

## Voorbeelden

Toont hoe VBA-referenties gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Zie ook

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


