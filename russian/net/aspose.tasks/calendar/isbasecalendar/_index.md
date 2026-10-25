---
title: "Calendar.IsBaseCalendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Calendar. Возвращает значение, указывающее, является ли календарь базовым"
type: docs
weight: 70
url: /ru/net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

Получает значение, указывающее, является ли календарь базовым.

```csharp
public bool IsBaseCalendar { get; }
```

## Примеры

Показывает, как читать календари проекта и их свойства.

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // Показывает, есть ли базовый календарь.
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // Получить время в часах за каждый рабочий день.
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


