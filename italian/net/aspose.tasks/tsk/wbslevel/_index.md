---
title: "Tsk.WBSLevel"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il livello WBS più a destra di un'attività"
type: docs
weight: 1140
url: /it/net/aspose.tasks/tsk/wbslevel/
---
## Tsk.WBSLevel field

Il livello WBS più a destra di un'attività.

```csharp
public static readonly Key<string, TaskKey> WBSLevel;
```

## Esempi

Mostra come leggere i codici WBS dell'attività.

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizza tutti i task raccolti
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


