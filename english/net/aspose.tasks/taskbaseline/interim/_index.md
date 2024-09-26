---
title: TaskBaseline.Interim
second_title: Aspose.Tasks for .NET API Reference
description: TaskBaseline property. Gets or sets a value indicating whether this is an Interim Baseline
type: docs
weight: 60
url: /net/aspose.tasks/taskbaseline/interim/
---
## TaskBaseline.Interim property

Gets or sets a value indicating whether this is an Interim Baseline.

```csharp
public bool Interim { get; set; }
```

## Examples

Shows how to get access to a baseline information.

```csharp
var project = new Project();

// Creating TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Display task baseline duration
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// value indicating whether this is an Interim Baseline
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// print timephased data of task baseline
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### See Also

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


