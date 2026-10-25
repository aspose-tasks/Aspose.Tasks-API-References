---
title: "ChildTasksCollector.Alg"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ChildTasksCollector methode. Verwerkt het opgegeven object"
type: docs
weight: 30
url: /nl/net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

Verwerkt het opgegeven object.

```csharp
public override void Alg(Task el, int level)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | Taak | Object om te verwerken. |
| niveau | Int32 | Boomknoopniveau. |

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


