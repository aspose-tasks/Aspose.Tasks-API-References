---
title: Project.DefaultWeekWorkingDays
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets the instance of WeekDayCollection class which represents a collection of project default week working days and working times
type: docs
weight: 370
url: /net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

Gets the instance of [`WeekDayCollection`](../../weekdaycollection/) class which represents a collection of project default week working days and working times.

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### Return Value

The instance of [`WeekDayCollection`](../../weekdaycollection/) class which contains a list of [`WeekDay`](../../weekday/) objects.

## Remarks

The data contains only in mpp files (not in xml).

## Examples

Shows how to get default week working day.

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### See Also

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


