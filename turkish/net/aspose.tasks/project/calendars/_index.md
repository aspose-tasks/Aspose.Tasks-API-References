---
title: "Project.Calendars"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Bu Project örneğinin CalendarCollection nesnesini alır."
type: docs
weight: 130
url: /tr/net/aspose.tasks/project/calendars/
---
## Project.Calendars property

Bu Project örneğinin [`CalendarCollection`](../../calendarcollection/) nesnesini alır.

```csharp
public CalendarCollection Calendars { get; }
```

## Örnekler

Proje takvimlerini nasıl okuyacağınızı gösterir.

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

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


