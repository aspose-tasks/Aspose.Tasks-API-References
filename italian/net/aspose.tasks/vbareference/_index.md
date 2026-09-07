---
title: "Classe VbaReference"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.VbaReference classe. Rappresenta un riferimento del VbaProject"
type: docs
weight: 2870
url: /it/net/aspose.tasks/vbareference/
---
## VbaReference class

Rappresenta un riferimento del [`VbaProject`](../vbaproject/).

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [VbaReference](vbareference/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | Ottiene l'identificatore della libreria. |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | Ottiene o imposta il nome del riferimento VBA. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | Restituisce un valore che indica se questa istanza è uguale all'oggetto `VbaReference` specificato. |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | Restituisce un valore che indica se questa istanza è uguale all'oggetto `VbaReference` specificato. |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | Restituisce un valore di hash code per questo `VbaReference`. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


