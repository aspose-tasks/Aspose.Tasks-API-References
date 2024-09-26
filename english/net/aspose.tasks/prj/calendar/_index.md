---
title: Prj.Calendar
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The project calendar
type: docs
weight: 90
url: /net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

The project calendar.

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## Examples

Shows how to read/write Prj.Calendar property.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

project.Set(Prj.Calendar, calendar);

Console.WriteLine("Calendar: " + project.Get(Prj.Calendar).Name);
foreach (var weekDay in calendar.WeekDays)
{
    Console.WriteLine(weekDay.FromDate);
    Console.WriteLine(weekDay.ToDate);
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


