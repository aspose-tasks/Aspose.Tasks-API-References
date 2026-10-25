---
title: "Rsc.CostPerUse"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il costo che si accumula ogni volta che una risorsa viene utilizzata"
type: docs
weight: 240
url: /it/net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

Il costo che si accumula ogni volta che una risorsa viene utilizzata.

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.CostPerUse.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


