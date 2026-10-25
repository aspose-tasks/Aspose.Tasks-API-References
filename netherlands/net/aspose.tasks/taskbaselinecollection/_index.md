---
title: "Klasse TaskBaselineCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TaskBaselineCollection klasse. Stelt een verzameling van TaskBaseline-objecten voor"
type: docs
weight: 2380
url: /nl/net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

Stelt een verzameling van [`TaskBaseline`](../taskbaseline/) objecten voor.

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | Haalt het aantal objecten op dat in dit TaskBaselineCollection-object zit. |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | Retourneert het element op de opgegeven index. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | Dit is de stub-implementatie van de Add-methode van ICollection, die alleen NotSupportedException gooit. |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | Verwijdert de baseline uit deze collectie. |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | Converteert het TaskBaselineCollection-object naar een lijst van [`TaskBaseline`](../taskbaseline/) objecten. |

## Voorbeelden

Toont hoe te werken met taakbaseline-collecties.

```csharp
var project = new Project();

// maak projectbaselines
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// print taakbaselines
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// Laten we alle basislijnen wissen
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### Zie ook

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


