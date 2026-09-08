---
title: "Task.Baselines"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Taakeigenschap. Haalt de collectie van baseline‑waarden van de taak op of stelt deze in."
type: docs
weight: 130
url: /nl/net/aspose.tasks/task/baselines/
---
## Task.Baselines property

Haalt op of stelt de collectie van baseline-waarden van de taak in.

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## Voorbeelden

Toont hoe de baselines van een taak gelezen kunnen worden.

```csharp
var project = new Project();

// stel een baseline in
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Taakbasislangeduur weergeven
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### Zie ook

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


