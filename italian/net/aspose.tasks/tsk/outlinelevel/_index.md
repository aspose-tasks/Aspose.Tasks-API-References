---
title: "Tsk.OutlineLevel"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il livello di outline di un'attività"
type: docs
weight: 840
url: /it/net/aspose.tasks/tsk/outlinelevel/
---
## Tsk.OutlineLevel field

Il livello di struttura di un'attività.

```csharp
public static readonly Key<int, TaskKey> OutlineLevel;
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


