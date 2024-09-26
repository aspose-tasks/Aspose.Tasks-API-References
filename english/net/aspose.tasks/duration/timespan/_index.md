---
title: Duration.TimeSpan
second_title: Aspose.Tasks for .NET API Reference
description: Duration property. Gets TimeSpan instance of this Duration object. The TimeSpan instance of this Duration object
type: docs
weight: 40
url: /net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

Gets `TimeSpan` instance of this Duration object. The TimeSpan instance of this Duration object.

```csharp
public TimeSpan TimeSpan { get; }
```

## Examples

Shows how to convert a duration to a time span.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// get the task duration
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### See Also

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


