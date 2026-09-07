---
title: "Rsc.Code"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il codice o altre informazioni su una risorsa"
type: docs
weight: 210
url: /it/net/aspose.tasks/rsc/code/
---
## Rsc.Code field

Il codice o altre informazioni su una risorsa.

```csharp
public static readonly Key<string, RscKey> Code;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Code.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


