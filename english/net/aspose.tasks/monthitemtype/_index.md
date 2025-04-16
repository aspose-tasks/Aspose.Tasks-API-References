---
title: Enum MonthItemType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.MonthItemType enum. Specifies the month item for which an exception recurrence is scheduled
type: docs
weight: 1040
url: /net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

Specifies the month item for which an exception recurrence is scheduled.

```csharp
public enum MonthItemType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Indicates Undefined month item type. |
| Day | `0` | Indicates Day month item type. |
| Weekday | `1` | Indicates Weekday month item type. |
| WeekendDay | `2` | Indicates WeekendDay month item type. |
| Sunday | `3` | Indicates Sunday month item type. |
| Monday | `4` | Indicates Monday month item type. |
| Tuesday | `5` | Indicates Tuesday month item type. |
| Wednesday | `6` | Indicates Wednesday month item type. |
| Thursday | `7` | Indicates Thursday month item type. |
| Friday | `8` | Indicates Friday month item type. |
| Saturday | `9` | Indicates Saturday month item type. |

## Examples

Shows how to define calendar exception by month day.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// create a calendar
var calendar = project.Calendars.Add("Calendar1");

// create calendar exception for every friday
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// check that aa friday is exceptional
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// add the exception to the calendar
calendar.Exceptions.Add(exception);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


