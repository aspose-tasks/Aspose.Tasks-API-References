---
title: Calendar.IsBaseCalendar
second_title: Aspose.Tasks for .NET API Reference
description: Calendar property. Gets a value indicating whether the calendar is a base calendar
type: docs
weight: 70
url: /net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

Gets a value indicating whether the calendar is a base calendar.

```csharp
public bool IsBaseCalendar { get; }
```

## Examples

Shows how to read project calendars and their properties.

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // Show if it is has a base calendar
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // Get Time in hours on each working day
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


