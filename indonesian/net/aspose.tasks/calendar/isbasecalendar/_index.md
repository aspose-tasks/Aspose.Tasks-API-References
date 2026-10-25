---
title: "Calendar.IsBaseCalendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Calendar. Mendapatkan nilai yang menunjukkan apakah kalender adalah kalender dasar"
type: docs
weight: 70
url: /id/net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

Mendapatkan nilai yang menunjukkan apakah kalender adalah kalender dasar.

```csharp
public bool IsBaseCalendar { get; }
```

## Contoh

Menampilkan cara membaca kalender proyek dan propertinya.

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // Tampilkan apakah memiliki kalender dasar.
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // Dapatkan waktu dalam jam pada setiap hari kerja.
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


