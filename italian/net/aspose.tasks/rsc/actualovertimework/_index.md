---
title: "Rsc.ActualOvertimeWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La quantità effettiva di lavoro straordinario già svolto dalla risorsa assegnata alle attività"
type: docs
weight: 50
url: /it/net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

La quantità effettiva di lavoro straordinario già eseguita dalla risorsa assegnata alle attività.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


