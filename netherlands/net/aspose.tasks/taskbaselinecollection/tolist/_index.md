---
title: "TaskBaselineCollection.ToList"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskBaselineCollection methode. Converteert het TaskBaselineCollection-object naar een lijst van TaskBaseline-objecten"
type: docs
weight: 60
url: /nl/net/aspose.tasks/taskbaselinecollection/tolist/
---
## TaskBaselineCollection.ToList method

Converteert het TaskBaselineCollection-object naar een lijst van [`TaskBaseline`](../../taskbaseline/) objecten.

```csharp
public List<TaskBaseline> ToList()
```

### Retourwaarde

Lijst van [`TaskBaseline`](../../taskbaseline/) objecten.

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

* class [TaskBaseline](../../taskbaseline/)
* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


