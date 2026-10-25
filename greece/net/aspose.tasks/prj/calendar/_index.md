---
title: "Prj.Calendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Το ημερολόγιο του έργου"
type: docs
weight: 90
url: /el/net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

Το ημερολόγιο του έργου.

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.Calendar.

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

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


