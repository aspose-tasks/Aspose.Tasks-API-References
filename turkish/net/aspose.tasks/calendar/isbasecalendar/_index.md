---
title: "Calendar.IsBaseCalendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar özelliği. Takvimin temel takvim olup olmadığını gösteren bir değer alır"
type: docs
weight: 70
url: /tr/net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

Takvimin temel takvim olup olmadığını gösteren bir değeri alır.

```csharp
public bool IsBaseCalendar { get; }
```

## Örnekler

Proje takvimlerini ve özelliklerini okumanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // Bir temel takvime sahip olup olmadığını göster.
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // Her çalışma gününde saat cinsinden zamanı al.
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


