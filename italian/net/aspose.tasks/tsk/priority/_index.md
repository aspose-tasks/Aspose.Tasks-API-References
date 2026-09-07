---
title: "Tsk.Priority"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il livello di importanza assegnato a un'attività che a sua volta indica quanto facilmente un'attività o un'assegnazione può essere ritardata o suddivisa durante il livellamento delle risorse."
type: docs
weight: 930
url: /it/net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

Il livello di importanza attribuito a un'attività, che a sua volta indica quanto facilmente un'attività o un'assegnazione può essere ritardata o suddivisa durante il livellamento delle risorse.

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## Esempi

Mostra come leggere la priorità di un'attività.

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Visualizza le priorità per tutte le attività
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


