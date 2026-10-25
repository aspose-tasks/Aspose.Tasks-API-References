---
title: "Rsc.Type"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il tipo di una risorsa"
type: docs
weight: 660
url: /it/net/aspose.tasks/rsc/type/
---
## Rsc.Type field

Il tipo di una risorsa.

```csharp
public static readonly Key<ResourceType, RscKey> Type;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Type.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Type, ResourceType.Work);

Console.WriteLine("Type: " + resource.Get(Rsc.Type));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ResourceType](../../resourcetype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


