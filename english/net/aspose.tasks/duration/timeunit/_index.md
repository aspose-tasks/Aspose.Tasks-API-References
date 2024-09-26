---
title: Duration.TimeUnit
second_title: Aspose.Tasks for .NET API Reference
description: Duration property. Gets time unit type for this object. The time unit type of this Duration instance
type: docs
weight: 50
url: /net/aspose.tasks/duration/timeunit/
---
## Duration.TimeUnit property

Gets time unit type for this object. The time unit type of this Duration instance.

```csharp
public TimeUnitType TimeUnit { get; }
```

## Examples

Shows how to update a duration of tasks.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// get a task
var task1 = project.RootTask.Children.GetById(1);

// update the task duration
var duration1 = task1.Get(Tsk.Duration);

// add one day to the task 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// set a new duration to the task
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// get another task
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// change the duration by using actual time unit type
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// set a new duration to the task
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### See Also

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


