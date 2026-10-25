---
title: "Klasse WorkWeek"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WorkWeek klasse. Vertegenwoordigt de WorkWeek‑klasse."
type: docs
weight: 3640
url: /nl/net/aspose.tasks/workweek/
---
## WorkWeek class

Stelt WorkWeek-klasse voor.

```csharp
public class WorkWeek
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [WorkWeek](workweek/)() | Initialiseert een nieuw exemplaar van de `WorkWeek` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [FromDate](../../aspose.tasks/workweek/fromdate/) { get; set; } | Haalt op of stelt de start‑DateTime van de werkweek in. |
| [Name](../../aspose.tasks/workweek/name/) { get; set; } | Haalt op of stelt de Naam van de werkweek in. |
| [ToDate](../../aspose.tasks/workweek/todate/) { get; set; } | Haalt op of stelt de Eind‑DateTime van de werkweek in. |
| [WeekDays](../../aspose.tasks/workweek/weekdays/) { get; } | Haalt weekdagen op. |

## Voorbeelden

Toont hoe werkweekinformatie uit het project te lezen is.

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
    // Toon de naam van de werkweek, de naam van de bovenliggende kalender, van‑ en tot‑datums.
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // Deze gegevens gaan over de knop \"Details.\" waarmee je speciale werktijden kunt instellen voor een speciale weekdag of deze zelfs niet-werkend kunt maken
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // Je kunt verder door werktijden navigeren en deze weergeven
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }

    Console.WriteLine();
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


