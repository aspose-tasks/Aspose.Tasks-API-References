---
title: "TaskUtils.Apply"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskUtils-methode. Past het opgegeven algoritme toe op elke taak in een boom"
type: docs
weight: 10
url: /nl/net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

Past het opgegeven algoritme toe op elke taak van een boom.

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| root | Taak | Wortel van de boom |
| alg | ITreeAlgorithm`1 | Toegepast algoritme. |
| niveau | Int32 | Niveau van de worteltaak. |

## Voorbeelden

Toont hoe te werken met een boom‑algoritme.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// verzamel alle projecttaken
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// werk met taken alsof het een eenvoudige lijst is
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### Zie ook

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


