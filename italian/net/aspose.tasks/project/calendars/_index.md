---
title: "Project.Calendars"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Project. Ottiene l'oggetto CalendarCollection di questa istanza di Project."
type: docs
weight: 130
url: /it/net/aspose.tasks/project/calendars/
---
## Project.Calendars property

Ottiene l'oggetto [`CalendarCollection`](../../calendarcollection/) di questa istanza di Project.

```csharp
public CalendarCollection Calendars { get; }
```

## Esempi

Mostra come leggere i calendari del progetto.

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

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


