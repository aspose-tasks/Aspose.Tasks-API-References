---
title: "Rsc.Guid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Contiene il codice di identificazione unico generato per la risorsa"
type: docs
weight: 310
url: /it/net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

Contiene il codice di identificazione unico generato per la risorsa.

```csharp
public static readonly Key<string, RscKey> Guid;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Guid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


