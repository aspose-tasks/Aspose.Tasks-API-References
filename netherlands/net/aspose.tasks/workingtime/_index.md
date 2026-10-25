---
title: "Klasse WorkingTime"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WorkingTime klasse. Vertegenwoordigt een werktijd gedurende een weekdag"
type: docs
weight: 3660
url: /nl/net/aspose.tasks/workingtime/
---
## WorkingTime class

Stelt een werktijd tijdens een weekdag voor.

```csharp
public class WorkingTime
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | Initialiseert een nieuw exemplaar van de `WorkingTime` klasse met een interval met de opgegeven start- en eindtijden. |
| [WorkingTime](workingtime/#constructor)(int, int) | Initialiseert een nieuw exemplaar van de `WorkingTime` klasse met een intervalitem met de opgegeven start- en eindtijden. |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | Initialiseert een nieuw exemplaar van de `WorkingTime` klasse met een intervalitem met de opgegeven start- en eindtijden. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | Haalt het begin van een werktijd op. |
| [To](../../aspose.tasks/workingtime/to/) { get; } | Haalt het einde van een werktijd op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | Controleert of de objecten gelijk zijn. |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | Retourneert een hashcode-waarde voor het exemplaar van de `WorkingTime` klasse. |

## Voorbeelden

Toont hoe te werken met werktijdinformatie.

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // Deze gegevens gaan over de knop \"Details.\" waarmee je speciale werktijden kunt instellen voor een speciale weekdag of deze zelfs niet-werkend kunt maken
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
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
}

public static Calendar CreateCalendar(Project project)
{
    var calendar = project.Calendars.Add("MyCalendar", project.Calendars.GetByName("Standard"));
    var workingTimes = new List<WorkingTime>
                           {
                               new WorkingTime(new DateTime(1, 1, 1, 9, 0, 0), new DateTime(1, 1, 1, 12, 0, 0)),
                               new WorkingTime(new DateTime(1, 1, 1, 13, 0, 0), new DateTime(1, 1, 1, 18, 0, 0))
                           };

    calendar.WeekDays.Add(new WeekDay(DayType.Monday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Wednesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Thursday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Friday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
    calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

    return calendar;
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


