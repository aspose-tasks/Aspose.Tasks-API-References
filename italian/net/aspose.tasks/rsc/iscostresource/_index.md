---
title: "Rsc.IsCostResource"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Determina se una risorsa è una risorsa di costo"
type: docs
weight: 390
url: /it/net/aspose.tasks/rsc/iscostresource/
---
## Rsc.IsCostResource field

Determina se una risorsa è una risorsa di costo.

```csharp
public static readonly Key<NullableBool, RscKey> IsCostResource;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.IsCostResource.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsCostResource, true);

Console.WriteLine("Is Cost Resource: " + resource.Get(Rsc.IsCostResource));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


