---
title: Class TaskBaseline
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TaskBaseline class. Represents Baseline of a Task
type: docs
weight: 2350
url: /net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

Represents Baseline of a Task.

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## Constructors

| Name | Description |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | Initializes a new instance of the `TaskBaseline` class. |

## Properties

| Name | Description |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Gets or sets the unique number of a baseline data record. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Gets or sets the budgeted cost of a work performed by a resource for a project to-date. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Gets or sets the budget cost of a work scheduled for a resource. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Gets or sets the projected cost of a resource when the baseline is saved. |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | Gets or sets the scheduled duration of the task when the baseline was saved. |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | Gets or sets a value indicating whether the baseline duration of the task was estimated. |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | Gets or sets the scheduled finish date of the task when the baseline was saved. |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | Gets or sets a fixed cost of the task when the baseline was saved. |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | Gets or sets a value indicating whether this is an Interim Baseline. |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | Gets or sets the scheduled start date of the task when the baseline was saved. |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | Gets or sets a TimephasedDataCollection instance for this object. The time phased data associated with the task baseline. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Gets or sets the work assigned to a resource when the baseline is saved. The amount of assigned work to a resource when the baseline was saved. |

## Methods

| Name | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable interface implementation. Compares this instance to the specified Baseline object. |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | IComparable interface implementation. Compares this instance to the specified Baseline object. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Returns a value indicating whether this instance is equal to a specified object. |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | Returns a value indicating whether this instance is equal to the specified TaskBaseline object. |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | Returns a hash code value for the instance of the `TaskBaseline` class. |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


