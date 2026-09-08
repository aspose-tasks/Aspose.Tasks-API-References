---
title: "TaskBaselineCollection.Count"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskBaselineCollection-eigenschap. Haalt het aantal objecten op dat in dit TaskBaselineCollection-object is opgenomen."
type: docs
weight: 10
url: /nl/net/aspose.tasks/taskbaselinecollection/count/
---
## TaskBaselineCollection.Count property

Haalt het aantal objecten op dat in dit TaskBaselineCollection-object zit.

```csharp
public int Count { get; }
```

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

* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


