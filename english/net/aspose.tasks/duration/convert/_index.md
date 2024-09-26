---
title: Duration.Convert
second_title: Aspose.Tasks for .NET API Reference
description: Duration method. Converts Duration object to another duration with specified time units
type: docs
weight: 70
url: /net/aspose.tasks/duration/convert/
---
## Duration.Convert method

Converts Duration object to another duration with specified time units.

```csharp
public Duration Convert(TimeUnitType timeUnitType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| timeUnitType | TimeUnitType | the specified time unit type. |

### Return Value

returns new duration with the specified unit type.

## Examples

Shows how to convert a duration into different time unit types.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Get a task to calculate its duration in different formats
var task = project.RootTask.Children.GetById(1);

// Get the duration in Minutes, Days, Hours, Weeks and Months
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### See Also

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


