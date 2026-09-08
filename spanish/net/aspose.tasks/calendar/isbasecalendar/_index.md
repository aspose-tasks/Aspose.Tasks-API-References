---
title: "Calendar.IsBaseCalendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Calendar. Obtiene un valor que indica si el calendario es un calendario base"
type: docs
weight: 70
url: /es/net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

Obtiene un valor que indica si el calendario es un calendario base.

```csharp
public bool IsBaseCalendar { get; }
```

## Ejemplos

Muestra cómo leer los calendarios del proyecto y sus propiedades.

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

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


