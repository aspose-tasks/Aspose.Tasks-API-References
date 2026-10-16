---
title: Project.SetBaseline
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Saves baseline fields to the specified baseline for the entire project
type: docs
weight: 1250
url: /net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

Saves baseline fields to the specified baseline for the entire project.

```csharp
public void SetBaseline(BaselineType baselineType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | BaselineType | The baseline type to save baseline data to. |

## Examples

Shows how to create baselines for a whole project.

```csharp
var project = new Project();

// Adding tasks
var task = project.RootTask.Children.Add("Task");
task.Work = project.GetDuration(TimeSpan.FromHours(8), TimeUnitType.Day);
var task2 = project.RootTask.Children.Add("Task2");

// Set project's baseline with type 'Baseline'
project.SetBaseline(BaselineType.Baseline);

var baseline = task.Baselines[0];

Console.WriteLine("Baseline start: {0}", baseline.Start);
Console.WriteLine("Baseline finish: {0}", baseline.Finish);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline timephased data:");

foreach (var td in baseline.TimephasedData)
{
    Console.WriteLine("[{0}] {1} - {2}, {3}", td.TimephasedDataType, td.Start, td.Finish, td.Value);
}
```

### See Also

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

Saves baseline fields to the specified baseline for the selected tasks.

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | BaselineType | The baseline type to save baseline data to. |
| taskCollection | IEnumerable`1 | List of tasks to save baseline data for. |

## Examples

Shows how to create set baselines for specific tasks.

```csharp
var project = new Project();

// Adding tasks
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// Set baseline for specified tasks
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### See Also

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


