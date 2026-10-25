---
title: "Rsc.RemainingOvertimeWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La quantità di straordinario programmato rimanente"
type: docs
weight: 600
url: /it/net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

L'importo del restante straordinario programmato.

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


