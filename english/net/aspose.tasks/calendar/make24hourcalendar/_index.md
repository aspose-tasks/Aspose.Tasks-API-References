---
title: Calendar.Make24HourCalendar
second_title: Aspose.Tasks for .NET API Reference
description: Calendar method. Makes a given Calendar to be a 24Hour Calendar. 24Hours Calendar is a Calendar in which every day of week is working with Roundtheclock working hours
type: docs
weight: 10
url: /net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

Makes a given Calendar to be a 24Hour Calendar. 24Hours Calendar is a Calendar in which every day of week is working with Round-the-clock working hours.

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| Parameter | Type | Description |
| --- | --- | --- |
| calendar | Calendar | Calendar to make 24 Hours Calendar from. |

### Return Value

24Hour Calendar.

## Examples

Shows how to create a 24 hours calendar.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24 hours will be printed
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

Shows how to transform a new calendar into a 24 hours calendar.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24 hours will be printed
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


