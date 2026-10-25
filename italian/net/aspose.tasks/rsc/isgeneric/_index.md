---
title: "Rsc.IsGeneric"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Determina se una risorsa è generica o meno"
type: docs
weight: 410
url: /it/net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

Determina se una risorsa è generica o meno.

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.IsGeneric.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


