---
title: Enum CalendarExceptionType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.CalendarExceptionType enum. Specifies the calendar exception type
type: docs
weight: 270
url: /net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

Specifies the calendar exception type.

```csharp
public enum CalendarExceptionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Daily | `0` | Indicates Daily exception type. |
| YearlyByDay | `1` | Indicates Yearly by day of the month exception type. |
| YearlyByPosition | `2` | Indicates Yearly by position exception type. |
| MonthlyByDay | `3` | Indicates Monthly by day of the month exception type. |
| MonthlyByPosition | `4` | Indicates Monthly by position exception type. |
| Weekly | `5` | Indicates Weekly exception type. |
| ByDayCount | `6` | Indicates By day count exception type. |
| ByWeekDayCount | `7` | Indicates By weekday count exception type. |
| NoExceptionType | `8` | Indicates No exception type. |

## Examples

Shows how to define a calendar exception by occurrences.

```csharp
var project = new Project();

// Define a calendar
var calendar = project.Calendars.Add("Calendar1");

// Define exception and specify occurrences
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// Add exception to calendar
calendar.Exceptions.Add(exception);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


