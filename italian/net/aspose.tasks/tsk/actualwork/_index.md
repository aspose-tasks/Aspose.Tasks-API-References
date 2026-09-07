---
title: "Tsk.ActualWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La quantità di lavoro già svolta dalle risorse assegnate ai compiti"
type: docs
weight: 90
url: /it/net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

La quantità di lavoro già svolta dalle risorse assegnate alle attività.

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


