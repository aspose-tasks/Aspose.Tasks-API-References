---
title: Duration.ToString
second_title: Aspose.Tasks for .NET API Reference
description: Duration method. Returns a string representation of this instance
type: docs
weight: 120
url: /net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

Returns a string representation of this instance.

```csharp
public override string ToString()
```

### Return Value

a string representation of this instance.

## Examples

Shows how to convert a duration to a string.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// get the task duration
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### See Also

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


