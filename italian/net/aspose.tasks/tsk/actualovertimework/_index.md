---
title: "Tsk.ActualOvertimeWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La quantità effettiva di lavoro straordinario già svolto dalle risorse assegnate alle attività"
type: docs
weight: 60
url: /it/net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

La quantità effettiva di lavoro straordinario già eseguito dalle risorse assegnate alle attività.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


