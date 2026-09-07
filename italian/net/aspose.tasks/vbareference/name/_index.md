---
title: "VbaReference.Name"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà VbaReference. Ottiene o imposta il nome del riferimento VBA"
type: docs
weight: 30
url: /it/net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

Ottiene o imposta il nome del riferimento VBA.

```csharp
public string Name { get; set; }
```

## Esempi

Mostra come leggere i riferimenti VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Vedi anche

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


