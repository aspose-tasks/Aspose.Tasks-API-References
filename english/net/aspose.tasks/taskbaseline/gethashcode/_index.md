---
title: TaskBaseline.GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: TaskBaseline method. Returns a hash code value for the instance of the TaskBaseline class
type: docs
weight: 110
url: /net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

Returns a hash code value for the instance of the [`TaskBaseline`](../) class.

```csharp
public override int GetHashCode()
```

### Return Value

returns a hash code value for this object.

## Examples

Shows how to get hash code of a task baseline.

```csharp
var project = new Project();

// creating TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// display task baseline duration
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// the hash code of a calendar is equal to baseline number 
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### See Also

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


