---
title: "Rsc.CostVariance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La differenza tra il costo di base e il costo totale per una risorsa"
type: docs
weight: 250
url: /it/net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

La differenza tra il costo di base e il costo totale per una risorsa.

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.CostVariance.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


