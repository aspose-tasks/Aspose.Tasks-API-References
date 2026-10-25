---
title: "Rsc.CanLevel"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Determina se è possibile effettuare il livellamento delle risorse su una risorsa"
type: docs
weight: 200
url: /it/net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

Determina se il livellamento delle risorse può essere eseguito su una risorsa.

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.CanLevel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


