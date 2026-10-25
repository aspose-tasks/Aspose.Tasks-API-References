---
title: "TaskBaselineCollection.Remove"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskBaselineCollection methode. Verwijdert baseline uit deze collectie"
type: docs
weight: 50
url: /nl/net/aspose.tasks/taskbaselinecollection/remove/
---
## TaskBaselineCollection.Remove method

Verwijdert de baseline uit deze collectie.

```csharp
public bool Remove(TaskBaseline item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | TaskBaseline | Het item om te verwijderen. |

### Retourwaarde

true als het item succesvol is verwijderd; anders false

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


