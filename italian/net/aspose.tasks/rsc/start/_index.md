---
title: "Rsc.Start"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La data in cui una risorsa assegnata è programmata per iniziare a lavorare su un'attività"
type: docs
weight: 640
url: /it/net/aspose.tasks/rsc/start/
---
## Rsc.Start field

La data in cui una risorsa assegnata è programmata per iniziare a lavorare su un'attività.

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Start.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


