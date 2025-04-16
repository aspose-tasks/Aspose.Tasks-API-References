---
title: Enum MonthPosition
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.MonthPosition enum. Specifies the position of a month item within a month
type: docs
weight: 1060
url: /net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

Specifies the position of a month item within a month.

```csharp
public enum MonthPosition
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Indicates Undefined month position. |
| First | `0` | Indicates First position month position. |
| Second | `1` | Indicates Second position month position. |
| Third | `2` | Indicates Third position month position. |
| Fourth | `3` | Indicates Fourth position month position. |
| Last | `4` | Indicates Last position month position. |

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


