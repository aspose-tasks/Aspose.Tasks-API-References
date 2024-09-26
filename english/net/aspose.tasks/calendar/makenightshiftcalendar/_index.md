---
title: Calendar.MakeNightShiftCalendar
second_title: Aspose.Tasks for .NET API Reference
description: Calendar method. Makes a given Calendar as Night Shift Calendar
type: docs
weight: 20
url: /net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

Makes a given Calendar as Night Shift Calendar.

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| Parameter | Type | Description |
| --- | --- | --- |
| calendar | Calendar | Calendar to make Night Shift Calendar. |

### Return Value

Night Shift Calendar.

## Examples

Shows how to create a night shift calendar.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// show working hours
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Shows how to transform a calendar into a night shift calendar.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// show working hours
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


