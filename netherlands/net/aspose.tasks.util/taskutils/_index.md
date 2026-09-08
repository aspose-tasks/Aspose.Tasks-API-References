---
title: "Class TaskUtils"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Util.TaskUtils class. Helperklasse die nuttige bewerkingen met taken biedt"
type: docs
weight: 2770
url: /nl/net/aspose.tasks.util/taskutils/
---
## TaskUtils class

Helperklasse die nuttige bewerkingen met taken biedt.

```csharp
public static class TaskUtils
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | Past het opgegeven algoritme toe op elke taak van een boom. |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | Bouwt een nieuwe boom van taken die aan de voorwaarde voldoen. |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | Vindt een taak die aan de voorwaarde voldoet in een boom van taken. |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | Berekent recursief het aantal onderliggende taken van een taak over alle niveaus. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


