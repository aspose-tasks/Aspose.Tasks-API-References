---
title: "Rsc.Id"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. L'identificatore di posizione di una risorsa nell'elenco delle risorse"
type: docs
weight: 350
url: /it/net/aspose.tasks/rsc/id/
---
## Rsc.Id field

L'identificatore di posizione di una risorsa nell'elenco delle risorse.

```csharp
public static readonly Key<int, RscKey> Id;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Id.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


