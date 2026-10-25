---
title: "Rsc.Name"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il nome di una risorsa"
type: docs
weight: 460
url: /it/net/aspose.tasks/rsc/name/
---
## Rsc.Name field

Il nome di una risorsa.

```csharp
public static readonly Key<string, RscKey> Name;
```

## Esempi

Mostra come leggere/scrivere la proprietà **Rsc.Name**.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


