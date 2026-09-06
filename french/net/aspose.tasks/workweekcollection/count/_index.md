---
title: "WorkWeekCollection.Count"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété WorkWeekCollection. Obtient le nombre d'objets contenus dans cet objet WorkWeekCollection"
type: docs
weight: 10
url: /fr/net/aspose.tasks/workweekcollection/count/
---
## WorkWeekCollection.Count property

Obtient le nombre d'objets contenus dans cet objet [`WorkWeekCollection`](../).

```csharp
public int Count { get; }
```

## Exemples

Montre comment créer une semaine de travail personnalisée pour un calendrier.

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

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
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

* class [WorkWeekCollection](../)
* namespace [Aspose.Tasks](../../workweekcollection/)
* assembly [Aspose.Tasks](../../../)


