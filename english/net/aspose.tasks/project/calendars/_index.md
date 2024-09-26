---
title: Project.Calendars
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets CalendarCollection object of this Project instance
type: docs
weight: 130
url: /net/aspose.tasks/project/calendars/
---
## Project.Calendars property

Gets [`CalendarCollection`](../../calendarcollection/) object of this Project instance.

```csharp
public CalendarCollection Calendars { get; }
```

## Examples

Shows how to read project calendars.

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

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


