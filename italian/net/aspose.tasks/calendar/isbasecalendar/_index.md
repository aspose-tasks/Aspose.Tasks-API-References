---
title: "Calendar.IsBaseCalendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Calendar. Restituisce un valore che indica se il calendario è un calendario base"
type: docs
weight: 70
url: /it/net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

Ottiene un valore che indica se il calendario è un calendario base.

```csharp
public bool IsBaseCalendar { get; }
```

## Esempi

Mostra come leggere i calendari di progetto e le loro proprietà.

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // Mostra se ha un calendario di base.
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // Ottieni il tempo in ore per ogni giorno lavorativo.
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


