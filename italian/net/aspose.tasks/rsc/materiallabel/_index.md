---
title: "Rsc.MaterialLabel"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. L'unità di misura per la risorsa materiale"
type: docs
weight: 440
url: /it/net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

L'unità di misura per la risorsa materiale.

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.MaterialLabel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


