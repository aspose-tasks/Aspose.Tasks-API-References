---
title: Calendar.GetTaskFinishDateFromDuration
second_title: Aspose.Tasks for .NET API Reference
description: Calendar method. Calculates the task finish date and time from its start date split parts and the work duration
type: docs
weight: 200
url: /net/aspose.tasks/calendar/gettaskfinishdatefromduration/
---
## Calendar.GetTaskFinishDateFromDuration method

Calculates the task finish date and time from its start date, split parts and the work duration.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Parameter | Type | Description |
| --- | --- | --- |
| task | Task | The task to calculate finish date for. |
| duration | TimeSpan | The duration to calculate. |

### Return Value

Task's finish date for the given start date and duration.

## Remarks

Returns DateTime.MinValue if task is summary, null or its start date is not set.

## Examples

Shows how to calculate finish date of a task by a custom duration.

```csharp
var project = new Project(DataDir + "SplitTaskFinishDate.mpp");

// Find a split task
var task = project.RootTask.Children.GetByUid(4);

// Find the project calendar
var calendar = project.Get(Prj.Calendar);

// Calculate task's finish date with different durations
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 8 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(8, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 16 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(16, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 24 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(24, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 28 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(28, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 32 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(32, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 46 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(46, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 61 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(61, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 75 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(75, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 80 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(80, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 120 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(120, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 150 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(150, 0, 0)));
```

### See Also

* class [Task](../../task/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


