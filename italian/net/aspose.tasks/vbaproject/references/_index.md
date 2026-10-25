---
title: "VbaProject.References"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà VbaProject. Ottiene una raccolta di VbaReferenceCollection"
type: docs
weight: 70
url: /it/net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

Ottiene una raccolta di [`VbaReferenceCollection`](../../vbareferencecollection/)

```csharp
public VbaReferenceCollection References { get; }
```

## Esempi

Mostra come leggere le informazioni di riferimento del progetto VBA.

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

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


