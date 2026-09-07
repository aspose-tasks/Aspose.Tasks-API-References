---
title: "Rsc.RemainingWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il tempo ancora necessario per completare un'attività o un insieme di attività"
type: docs
weight: 610
url: /it/net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

Il tempo ancora necessario per completare un'attività o un insieme di attività.

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


