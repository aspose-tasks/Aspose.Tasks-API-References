---
title: "Tsk.OutlineNumber"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il numero che rappresenta la posizione di un'attività nella struttura gerarchica dell'outline"
type: docs
weight: 850
url: /it/net/aspose.tasks/tsk/outlinenumber/
---
## Tsk.OutlineNumber field

Il numero che rappresenta la posizione di un'attività nella struttura gerarchica.

```csharp
public static readonly Key<string, TaskKey> OutlineNumber;
```

## Esempi

Mostra come leggere le proprietà di outline dell'attività.

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizza tutti i task raccolti
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


