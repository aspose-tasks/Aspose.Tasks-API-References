---
title: "Project.Calendars"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan objek CalendarCollection dari instance Project ini."
type: docs
weight: 130
url: /id/net/aspose.tasks/project/calendars/
---
## Project.Calendars property

Mendapatkan objek [`CalendarCollection`](../../calendarcollection/) dari instance Project ini.

```csharp
public CalendarCollection Calendars { get; }
```

## Contoh

Menampilkan cara membaca kalender proyek.

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

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


