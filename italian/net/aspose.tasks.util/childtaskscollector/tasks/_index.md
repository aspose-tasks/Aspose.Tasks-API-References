---
title: "ChildTasksCollector.Tasks"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ChildTasksCollector. Ottiene un elenco delle attività degli oggetti figlio raccolte"
type: docs
weight: 20
url: /it/net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

Ottiene un elenco di oggetti figli raccolti (task).

```csharp
public List<Task> Tasks { get; }
```

## Esempi

Mostra come iterare su tutti i task di un progetto come una semplice lista.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizza tutti i task raccolti
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Vedi anche

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


