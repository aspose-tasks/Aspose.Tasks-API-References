---
title: "Rsc.Inactive"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Determina se una risorsa è stata resa inattiva da un utente con diritti amministrativi"
type: docs
weight: 360
url: /it/net/aspose.tasks/rsc/inactive/
---
## Rsc.Inactive field

Determina se una risorsa è stata resa inattiva da un utente con diritti amministrativi.

```csharp
public static readonly Key<NullableBool, RscKey> Inactive;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Inactive.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Inactive, true);

Console.WriteLine("Inactive: " + resource.Get(Rsc.Inactive));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


