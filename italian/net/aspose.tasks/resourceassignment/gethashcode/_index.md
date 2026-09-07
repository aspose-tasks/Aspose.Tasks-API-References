---
title: "ResourceAssignment.GetHashCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "ResourceAssignment metodo. Restituisce un valore di hash code per l'istanza della classe ResourceAssignment"
type: docs
weight: 710
url: /it/net/aspose.tasks/resourceassignment/gethashcode/
---
## ResourceAssignment.GetHashCode method

Restituisce un valore di hash code per l'istanza della classe [`ResourceAssignment`](../).

```csharp
public override int GetHashCode()
```

### Valore di ritorno

restituisce un valore di hash per questo oggetto.

## Esempi

Mostra come ottenere un hash code di un'assegnazione di risorsa.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(2);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(3);

// stampa gli hash code dell'assegnazione
Console.WriteLine("Resource Assignment 1 Hash Code: {0}", resourceAssignment1.GetHashCode());
Console.WriteLine("Resource Assignment 2 Hash Code: {0}", resourceAssignment2.GetHashCode());
```

### Vedi anche

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


