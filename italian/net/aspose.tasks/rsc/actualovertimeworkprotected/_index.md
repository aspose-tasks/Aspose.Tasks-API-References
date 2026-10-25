---
title: "Rsc.ActualOvertimeWorkProtected"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La quantità di lavoro attraverso la quale il lavoro straordinario reale è protetto"
type: docs
weight: 60
url: /it/net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

La quantità di lavoro attraverso la quale il lavoro straordinario effettivo è protetto.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.ActualOvertimeWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


