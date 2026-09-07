---
title: "VbaReference.LibIdentifier"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà VbaReference. Ottiene l'identificatore della libreria"
type: docs
weight: 20
url: /it/net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

Ottiene l'identificatore della libreria.

```csharp
public string LibIdentifier { get; }
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


