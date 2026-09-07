---
title: "Tsk.RemainingWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il tempo ancora necessario per completare un'attività o un insieme di attività"
type: docs
weight: 990
url: /it/net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

Il tempo ancora necessario per completare un'attività o un insieme di attività.

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


