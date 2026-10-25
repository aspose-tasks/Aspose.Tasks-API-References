---
title: "Classe WorkingTime"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.WorkingTime. Représente un temps de travail pendant un jour de semaine."
type: docs
weight: 3660
url: /fr/net/aspose.tasks/workingtime/
---
## WorkingTime class

Représente un temps de travail pendant un jour de la semaine.

```csharp
public class WorkingTime
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | Initialise une nouvelle instance de la classe `WorkingTime` avec un intervalle aux heures de début et de fin spécifiées. |
| [WorkingTime](workingtime/#constructor)(int, int) | Initialise une nouvelle instance de la classe `WorkingTime` avec un élément d'intervalle aux heures de début et de fin spécifiées. |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | Initialise une nouvelle instance de la classe `WorkingTime` avec un élément d'intervalle aux heures de début et de fin spécifiées. |

## Propriétés

| Nom | Description |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | Obtient le début d'un temps de travail. |
| [To](../../aspose.tasks/workingtime/to/) { get; } | Obtient la fin d'un temps de travail. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | Vérifie que les objets sont égaux. |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | Renvoie une valeur de code de hachage pour l'instance de la classe `WorkingTime`. |

## Exemples

Montre comment travailler avec les informations de temps de travail.

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // Ces données concernent le bouton \"Détails.\" vous pouvez définir des temps de travail spéciaux pour un jour de semaine spécial ou même le rendre non ouvrable.
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


