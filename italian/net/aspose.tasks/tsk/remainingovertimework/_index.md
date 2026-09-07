---
title: "Tsk.RemainingOvertimeWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La quantità di tempo di straordinario programmato rimanente."
type: docs
weight: 980
url: /it/net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

La quantità di tempo di straordinario programmato rimanente.

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


