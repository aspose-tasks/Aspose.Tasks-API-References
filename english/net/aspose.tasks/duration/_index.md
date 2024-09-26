---
title: Struct Duration
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Duration struct. Represents duration in a project
type: docs
weight: 470
url: /net/aspose.tasks/duration/
---
## Duration structure

Represents duration in a project.

```csharp
public struct Duration : IEquatable<Duration>
```

## Properties

| Name | Description |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | Gets a value indicating whether time unit is elapsed. The flag which determines whether this Duration instance is elapsed. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | Gets a value indicating whether time unit is estimated. The flag which determines whether this Duration instance is estimated. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | Gets [`TimeSpan`](./timespan/) instance of this Duration object. The TimeSpan instance of this Duration object. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | Gets time unit type for this object. The time unit type of this Duration instance. |

## Methods

| Name | Description |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | Converts the specified string to the instance of `Duration` struct. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | Adds specified double value to this duration. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | Adds specified duration to this duration. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Converts Duration object to another duration with specified time units. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | Returns a value indicating whether this instance is equal to a specified object. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | Returns a hash code value for this object. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | Subtracts specified double value from this duration instance. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | Subtracts specified duration from this duration instance. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Converts Duration object to Double value. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | Returns a string representation of this instance. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | Parses duration string in format "PT--H--M--S--". |
| [operator ==](../../aspose.tasks/duration/op_equality/) | Returns a value indicating whether this instance is equal to a specified object. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | Returns a value indicating whether this instance is not equal to a specified object. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


