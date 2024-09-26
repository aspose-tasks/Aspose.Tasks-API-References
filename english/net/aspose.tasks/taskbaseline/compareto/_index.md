---
title: TaskBaseline.CompareTo
second_title: Aspose.Tasks for .NET API Reference
description: TaskBaseline method. IComparable interface implementation. Compares this instance to the specified Baseline object
type: docs
weight: 90
url: /net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

IComparable interface implementation. Compares this instance to the specified Baseline object.

```csharp
public int CompareTo(TaskBaseline other)
```

| Parameter | Type | Description |
| --- | --- | --- |
| other | TaskBaseline | the specified Baseline object to compare this instance to. |

### Return Value

returns -1 if this instance is less than the specified object, 1 if this instance is greater than the specified object; otherwise returns 0

## Examples

Shows how to check equality of baselines.

```csharp
var project = new Project();

// creating TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// display task baseline duration
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// the equality of baselines is checked against to baseline's numbers.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### See Also

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


