---
title: "Rsc.Uid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. L'identificatore unico di una risorsa"
type: docs
weight: 670
url: /it/net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

L'identificatore univoco di una risorsa.

```csharp
public static readonly Key<int, RscKey> Uid;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Uid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


