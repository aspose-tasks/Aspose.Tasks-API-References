---
title: "Project.Calendars"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété du projet. Obtient l'objet CalendarCollection de cette instance de Project"
type: docs
weight: 130
url: /fr/net/aspose.tasks/project/calendars/
---
## Project.Calendars property

Obtient l'objet [`CalendarCollection`](../../calendarcollection/) de cette instance de Project.

```csharp
public CalendarCollection Calendars { get; }
```

## Exemples

Montre comment lire les calendriers du projet.

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

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


