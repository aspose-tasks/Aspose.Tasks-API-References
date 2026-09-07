---
title: "Rsc.ActualOvertimeCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Costi sostenuti per lavoro straordinario già eseguito sui compiti dalle risorse assegnate"
type: docs
weight: 40
url: /it/net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

Costi sostenuti per il lavoro straordinario già svolto sui task dalle risorse assegnate.

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.ActualOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


