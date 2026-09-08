---
title: "Project.Calendars"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad del proyecto. Obtiene el objeto CalendarCollection de esta instancia de Project"
type: docs
weight: 130
url: /es/net/aspose.tasks/project/calendars/
---
## Project.Calendars property

Obtiene el objeto [`CalendarCollection`](../../calendarcollection/) de esta instancia de Project.

```csharp
public CalendarCollection Calendars { get; }
```

## Ejemplos

Muestra cómo leer los calendarios del proyecto.

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // Muestra si tiene un calendario base
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // Obtén el tiempo en horas en cada día laborable
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### Ver también

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


