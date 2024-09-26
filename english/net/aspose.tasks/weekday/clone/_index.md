---
title: WeekDay.Clone
second_title: Aspose.Tasks for .NET API Reference
description: WeekDay method. Returns a deep copy of the week day
type: docs
weight: 80
url: /net/aspose.tasks/weekday/clone/
---
## WeekDay.Clone method

Returns a deep copy of the week day.

```csharp
public WeekDay Clone()
```

### Return Value

Returns the deep copy of the week day.

## Examples

Shows how to clone a week day.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var calendar = project.Calendars.GetByUid(1);
var weekDay1 = calendar.WeekDays[0];

// create a deep copy week day
var weekDay2 = weekDay1.Clone();

// the equality of calendars is checked against to weekday's properties:
// weekday.DayType
// weekday.DayWorking
// weekday.FromDate
// weekday.ToDate
// weekday.WorkingTimes
Console.WriteLine("WeekDay 1 Day Type: " + weekDay1.DayType);
Console.WriteLine("WeekDay 1 Day Working: " + weekDay1.DayWorking);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.FromDate);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.ToDate);
Console.WriteLine("WeekDay 1 WorkingTimes: " + weekDay1.WorkingTimes);
Console.WriteLine("WeekDay 2 Day Type: " + weekDay2.DayType);
Console.WriteLine("WeekDay 2 Day Working: " + weekDay2.DayWorking);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.FromDate);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.ToDate);
Console.WriteLine("WeekDay 2 WorkingTimes: " + weekDay2.WorkingTimes);
Console.WriteLine("Are weekdays equal: " + weekDay1.Equals(weekDay2));
Console.WriteLine("Are weekdays equal (by reference): " + ReferenceEquals(weekDay1, weekDay2));
```

### See Also

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


