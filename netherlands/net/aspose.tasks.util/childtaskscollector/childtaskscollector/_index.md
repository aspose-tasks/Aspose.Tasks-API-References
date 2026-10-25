---
title: "ChildTasksCollector.ChildTasksCollector"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ChildTasksCollector constructor. Initialiseert een nieuw exemplaar van de ChildTasksCollector-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

Initialiseert een nieuw exemplaar van de [`ChildTasksCollector`](../) klasse.

```csharp
public ChildTasksCollector()
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

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


