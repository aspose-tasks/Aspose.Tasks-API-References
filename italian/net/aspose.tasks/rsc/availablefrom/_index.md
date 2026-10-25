---
title: "Rsc.AvailableFrom"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La data di inizio in cui una risorsa è disponibile per il lavoro alle unità specificate per il periodo di tempo corrente"
type: docs
weight: 120
url: /it/net/aspose.tasks/rsc/availablefrom/
---
## Rsc.AvailableFrom field

La data di inizio in cui una risorsa è disponibile per il lavoro alle unità specificate per il periodo di tempo corrente.

```csharp
public static readonly Key<DateTime, RscKey> AvailableFrom;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.AvailableFrom.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableFrom, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available From: " + resource.Get(Rsc.AvailableFrom));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


