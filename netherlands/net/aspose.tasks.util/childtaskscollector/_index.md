---
title: "Klasse ChildTasksCollector"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Util.ChildTasksCollector-klasse. Verzamelt alle onderliggende taken"
type: docs
weight: 2690
url: /nl/net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

Verzamelt alle onderliggende taken.

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | Initialiseert een nieuw exemplaar van de `ChildTasksCollector`-klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | Haalt een lijst met verzamelde onderliggende objecten (taken) op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | Verwerkt het opgegeven object. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


