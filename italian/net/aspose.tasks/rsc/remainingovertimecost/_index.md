---
title: "Rsc.RemainingOvertimeCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La spesa di straordinario programmata rimanente per una risorsa"
type: docs
weight: 590
url: /it/net/aspose.tasks/rsc/remainingovertimecost/
---
## Rsc.RemainingOvertimeCost field

La spesa di straordinario programmata rimanente per una risorsa.

```csharp
public static readonly Key<decimal, RscKey> RemainingOvertimeCost;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.RemainingOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeCost, 3);

Console.WriteLine("Remaining Overtime Cost: " + resource.Get(Rsc.RemainingOvertimeCost));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


