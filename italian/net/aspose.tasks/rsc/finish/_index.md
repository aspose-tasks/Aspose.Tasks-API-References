---
title: "Rsc.Finish"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La data in cui una risorsa è programmata per completare il lavoro su tutte le attività assegnate"
type: docs
weight: 290
url: /it/net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

La data in cui una risorsa è programmata per completare il lavoro su tutte le attività assegnate.

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Finish.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


