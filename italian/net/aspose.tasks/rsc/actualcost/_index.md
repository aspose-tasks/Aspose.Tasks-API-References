---
title: "Rsc.ActualCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Costi sostenuti per il lavoro già eseguito dalle risorse sulle loro attività insieme a eventuali altri costi registrati associati all'attività"
type: docs
weight: 30
url: /it/net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

Costi sostenuti per il lavoro già svolto dalle risorse sui loro task, insieme a eventuali altri costi registrati associati al task.

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.ActualCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


