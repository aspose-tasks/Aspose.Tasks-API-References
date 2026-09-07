---
title: "Prj.Calendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Kalender proyek"
type: docs
weight: 90
url: /id/net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

Kalender proyek.

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.Calendar.

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

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


