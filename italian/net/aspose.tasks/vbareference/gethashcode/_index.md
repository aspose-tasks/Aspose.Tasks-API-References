---
title: "VbaReference.GetHashCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo VbaReference. Restituisce un valore di hash code per questo VbaReference"
type: docs
weight: 50
url: /it/net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

Restituisce un valore di hash code per questo [`VbaReference`](../).

```csharp
public override int GetHashCode()
```

### Valore di ritorno

Restituisce un valore di hash code per questo oggetto.

## Esempi

Mostra come ottenere un hash code di un riferimento VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// L'hash code di un riferimento è l'hash code del GUID interno del riferimento
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### Vedi anche

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


