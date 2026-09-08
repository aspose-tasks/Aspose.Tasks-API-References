---
title: "Prj.Calendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Календарь проекта"
type: docs
weight: 90
url: /ru/net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

Календарь проекта.

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## Примеры

Показывает, как читать/записывать свойство Prj.Calendar.

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

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


