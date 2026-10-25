---
title: "Rsc.ActualWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La quantità di lavoro già svolta dalla risorsa assegnata ai compiti"
type: docs
weight: 70
url: /it/net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

La quantità di lavoro già svolta dalla risorsa assegnata alle attività.

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


