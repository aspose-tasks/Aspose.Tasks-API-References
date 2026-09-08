---
title: "ChildTasksCollector.Tasks"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ChildTasksCollector eigenschap. Haalt een lijst met verzamelde taken van kindobjecten op"
type: docs
weight: 20
url: /nl/net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

Haalt een lijst met verzamelde onderliggende objecten (taken) op.

```csharp
public List<Task> Tasks { get; }
```

## Voorbeelden

Toont hoe je over alle taken in een project kunt itereren als een eenvoudige lijst.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Alle verzamelde taken doorlopen
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Zie ook

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


