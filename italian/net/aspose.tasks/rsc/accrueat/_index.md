---
title: "Rsc.AccrueAt"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Determina come e quando i costi standard e gli straordinari della risorsa devono essere addebitati o accantonati al costo di un compito"
type: docs
weight: 10
url: /it/net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

Determina come e quando i costi standard e gli straordinari delle risorse devono essere addebitati o accreditati al costo di un task.

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.AccrueAt.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


