---
title: "Prj.Calendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Proje takvimi"
type: docs
weight: 90
url: /tr/net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

Proje takvimi.

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## Örnekler

Prj.Calendar özelliğini okuma/yazma yöntemini gösterir.

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

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


