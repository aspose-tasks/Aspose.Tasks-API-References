---
title: "Calendar.IsBaseCalendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Calendar. Obtient une valeur indiquant si le calendrier est un calendrier de base"
type: docs
weight: 70
url: /fr/net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

Obtient une valeur indiquant si le calendrier est un calendrier de base.

```csharp
public bool IsBaseCalendar { get; }
```

## Exemples

Montre comment lire les calendriers de projet et leurs propriétés.

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // Affiche s'il possède un calendrier de base.
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // Obtenir le temps en heures pour chaque jour ouvrable.
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


