---
title: "Rsc.Initials"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Le iniziali di una risorsa"
type: docs
weight: 370
url: /it/net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

Le iniziali di una risorsa.

```csharp
public static readonly Key<string, RscKey> Initials;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Initials.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


