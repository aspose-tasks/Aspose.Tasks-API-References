---
title: "Classe WorkWeek"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.WorkWeek. Représente la classe WorkWeek"
type: docs
weight: 3640
url: /fr/net/aspose.tasks/workweek/
---
## WorkWeek class

Représente la classe WorkWeek

```csharp
public class WorkWeek
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WorkWeek](workweek/)() | Initialise une nouvelle instance de la classe `WorkWeek`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [FromDate](../../aspose.tasks/workweek/fromdate/) { get; set; } | Obtient ou définit la DateTime de début de la semaine de travail |
| [Name](../../aspose.tasks/workweek/name/) { get; set; } | Obtient ou définit le Nom de la semaine de travail |
| [ToDate](../../aspose.tasks/workweek/todate/) { get; set; } | Obtient ou définit la DateTime de fin de la semaine de travail |
| [WeekDays](../../aspose.tasks/workweek/weekdays/) { get; } | Obtient les jours de la semaine. |

## Exemples

Montre comment lire les informations de la semaine de travail depuis le projet.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // Affiche le nom de la semaine de travail, le nom du calendrier parent, les dates de début et de fin
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // Ces données concernent le bouton \"Détails.\" vous pouvez définir des temps de travail spéciaux pour un jour de semaine spécial ou même le rendre non ouvrable.
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // Vous pouvez parcourir davantage les temps de travail et les afficher.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }

    Console.WriteLine();
}
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


