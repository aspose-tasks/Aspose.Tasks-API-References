---
title: Enum BaselineType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.BaselineType enum. Specifies the baseline type used to calculate Variance values
type: docs
weight: 130
url: /net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

Specifies the baseline type used to calculate Variance values.

```csharp
public enum BaselineType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Indicates the field was not defined in original project file. |
| Baseline | `0` | Indicates Baseline type. |
| Baseline1 | `1` | Indicates Baseline1 type. |
| Baseline2 | `2` | Indicates Baseline2 type. |
| Baseline3 | `3` | Indicates Baseline3 type. |
| Baseline4 | `4` | Indicates Baseline4 type. |
| Baseline5 | `5` | Indicates Baseline5 type. |
| Baseline6 | `6` | Indicates Baseline6 type. |
| Baseline7 | `7` | Indicates Baseline7 type. |
| Baseline8 | `8` | Indicates Baseline8 type. |
| Baseline9 | `9` | Indicates Baseline9 type. |
| Baseline10 | `10` | Indicates Baseline10 type. |

## Remarks

While exporting into XML the Undefined values will be eliminated from resulting XML.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


