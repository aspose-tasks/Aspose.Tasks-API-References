---
title: "ChildTasksCollector.ChildTasksCollector"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore di ChildTasksCollector. Inizializza una nuova istanza della classe ChildTasksCollector"
type: docs
weight: 10
url: /it/net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

Inizializza una nuova istanza della classe [`ChildTasksCollector`](../).

```csharp
public ChildTasksCollector()
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

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


