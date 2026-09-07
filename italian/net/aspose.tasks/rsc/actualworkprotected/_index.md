---
title: "Rsc.ActualWorkProtected"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La quantità di lavoro attraverso la quale il lavoro effettivo è protetto"
type: docs
weight: 80
url: /it/net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

La quantità di lavoro attraverso la quale il lavoro effettivo è protetto.

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


