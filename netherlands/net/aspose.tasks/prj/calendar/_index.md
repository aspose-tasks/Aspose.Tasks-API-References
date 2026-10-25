---
title: "Prj.Calendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj veld. De projectkalender"
type: docs
weight: 90
url: /nl/net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

De projectkalender.

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## Voorbeelden

Toont hoe de eigenschap Prj.Calendar te lezen/schrijven.

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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


