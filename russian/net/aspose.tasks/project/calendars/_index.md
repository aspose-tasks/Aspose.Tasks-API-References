---
title: "Project.Calendars"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Получает объект CalendarCollection данного экземпляра Project."
type: docs
weight: 130
url: /ru/net/aspose.tasks/project/calendars/
---
## Project.Calendars property

Получает объект [`CalendarCollection`](../../calendarcollection/) данного экземпляра Project.

```csharp
public CalendarCollection Calendars { get; }
```

## Примеры

Показывает, как читать календари проекта.

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

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


