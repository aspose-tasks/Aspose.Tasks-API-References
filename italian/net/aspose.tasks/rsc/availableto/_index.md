---
title: "Rsc.AvailableTo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La data di fine in cui una risorsa è disponibile per il lavoro alle unità specificate per il periodo di tempo corrente"
type: docs
weight: 130
url: /it/net/aspose.tasks/rsc/availableto/
---
## Rsc.AvailableTo field

La data di fine in cui una risorsa è disponibile per il lavoro alle unità specificate per il periodo di tempo corrente.

```csharp
public static readonly Key<DateTime, RscKey> AvailableTo;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.AvailableTo.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableTo, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available To: " + resource.Get(Rsc.AvailableTo));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


