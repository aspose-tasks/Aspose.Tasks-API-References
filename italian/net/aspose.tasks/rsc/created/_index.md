---
title: "Rsc.Created"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La data e l'ora in cui una risorsa è stata aggiunta al progetto"
type: docs
weight: 260
url: /it/net/aspose.tasks/rsc/created/
---
## Rsc.Created field

La data e l'ora in cui una risorsa è stata aggiunta al progetto.

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Created.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


