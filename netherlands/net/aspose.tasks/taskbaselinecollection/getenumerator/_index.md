---
title: "TaskBaselineCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskBaselineCollection methode. Retourneert een enumerator voor deze collectie"
type: docs
weight: 40
url: /nl/net/aspose.tasks/taskbaselinecollection/getenumerator/
---
## TaskBaselineCollection.GetEnumerator method

Retourneert een enumerator voor deze collectie.

```csharp
public IEnumerator<TaskBaseline> GetEnumerator()
```

### Retourwaarde

een enumerator voor deze collectie.

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


