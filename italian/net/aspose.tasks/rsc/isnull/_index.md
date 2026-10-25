---
title: "Rsc.IsNull"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Determina se una risorsa è nulla"
type: docs
weight: 420
url: /it/net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

Determina se una risorsa è nulla.

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.IsNull.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


