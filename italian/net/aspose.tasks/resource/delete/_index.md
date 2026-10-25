---
title: "Resource.Delete"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo della risorsa. Elimina una risorsa e le sue assegnazioni dal progetto"
type: docs
weight: 810
url: /it/net/aspose.tasks/resource/delete/
---
## Resource.Delete method

Elimina una risorsa e le sue assegnazioni dal progetto.

```csharp
public void Delete()
```

## Esempi

Mostra come eliminare una risorsa.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// elimina la risorsa
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### Vedi anche

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


