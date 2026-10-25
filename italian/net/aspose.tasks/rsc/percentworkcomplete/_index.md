---
title: "Rsc.PercentWorkComplete"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La percentuale di lavoro completato su tutte le attività"
type: docs
weight: 550
url: /it/net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

La percentuale di lavoro completato su tutti i compiti.

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## Esempi

Mostra come leggere la percentuale di lavoro completato della risorsa.

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// Visualizza la percentuale di completamento del lavoro per tutte le risorse
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


