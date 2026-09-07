---
title: "Rsc.CostCenter"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Indica a quale centro di costo devono essere addebitati i costi accumulati dalla risorsa"
type: docs
weight: 230
url: /it/net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

Indica a quale centro di costo devono essere addebitati i costi accumulati dalla risorsa.

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.CostCenter.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


