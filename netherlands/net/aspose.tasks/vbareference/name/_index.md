---
title: "VbaReference.Name"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaReference-eigenschap. Haalt op of stelt de naam van de VBA-referentie in"
type: docs
weight: 30
url: /nl/net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

Haalt de naam van de VBA-referentie op of stelt deze in.

```csharp
public string Name { get; set; }
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


