---
title: "Project.RemoveInvalidResourceAssignments"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Project. Elimina le assegnazioni di risorse non valide dall'elenco delle assegnazioni di risorse del progetto."
type: docs
weight: 1170
url: /it/net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

Elimina le assegnazioni di risorse non valide dall'elenco delle assegnazioni di risorse del progetto.

```csharp
public void RemoveInvalidResourceAssignments()
```

## Osservazioni

MS Project crea un'assegnazione di risorsa vuota per ogni attività. Chiama il metodo per rimuoverle.

## Esempi

Mostra come rimuovere le assegnazioni non valide.

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// rimuovi assegnazioni non valide
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


