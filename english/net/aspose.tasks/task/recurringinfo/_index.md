---
title: Task.RecurringInfo
second_title: Aspose.Tasks for .NET API Reference
description: Task property. Gets the instance of RecurringTaskInfo class for the task which is a recurring task if the task is not a recurring one then returns null The info for the instance of RecurringTaskInfo is present in mpp file format only
type: docs
weight: 1030
url: /net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

Gets the instance of [`RecurringTaskInfo`](../../recurringtaskinfo/) class for the task which is a recurring task; if the task is not a recurring one then returns null; The info for the instance of [`RecurringTaskInfo`](../../recurringtaskinfo/) is present in mpp file format only.

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## Examples

Shows how to read task's recurring info.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Recurrence Pattern: " + task.RecurringInfo.RecurrencePattern);
Console.WriteLine("Start Date: " + task.RecurringInfo.StartDate);
Console.WriteLine("End Date: " + task.RecurringInfo.EndDate);
Console.WriteLine("Duration: " + task.RecurringInfo.Duration);
Console.WriteLine("Occurrences: " + task.RecurringInfo.Occurrences);
Console.WriteLine("Weekly Days: " + task.RecurringInfo.WeeklyDays);
Console.WriteLine("WeeklyRepetitions: " + task.RecurringInfo.WeeklyRepetitions);
```

### See Also

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


