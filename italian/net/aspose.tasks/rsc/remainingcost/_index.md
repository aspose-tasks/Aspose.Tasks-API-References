---
title: "Rsc.RemainingCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La spesa programmata residua che sarà sostenuta nel completare il lavoro programmato residuo"
type: docs
weight: 580
url: /it/net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

La spesa programmata rimanente che sarà sostenuta nel completare il lavoro programmato rimanente.

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.RemainingCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


