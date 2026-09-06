---
title: "WorkingTime.WorkingTime"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "constructeur WorkingTime. Initialise une nouvelle instance de la classe WorkingTime avec un intervalle aux heures de début et de fin spécifiées"
type: docs
weight: 10
url: /fr/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Initialise une nouvelle instance de la classe [`WorkingTime`](../) avec un intervalle aux heures de début et de fin spécifiées.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fromTime | DateTime | heure de début de l'intervalle |
| toTime | DateTime | heure de fin de l'intervalle |

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

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Initialise une nouvelle instance de la classe [`WorkingTime`](../) avec un élément d'intervalle aux heures de début et de fin spécifiées.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fromTime | TimeSpan | Heure de début de l'intervalle représentée par la structure TimeSpan. |
| toTime | TimeSpan | Heure de fin de l'intervalle représentée par la structure TimeSpan. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Lorsque toTime est inférieur ou égal à l'argument toTime ou lorsque l'intervalle entre fromTime et toTime dépasse 24 heures. |

## Exemples

La surcharge du constructeur WorkingTime peut être utilisée pour initialiser le début et la fin de l'intervalle à l'aide de TimeSpans :

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### Voir aussi

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Initialise une nouvelle instance de la classe [`WorkingTime`](../) avec un élément d'intervalle aux heures de début et de fin spécifiées.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fromHours | Int32 | Heure de début de l'intervalle représentée par un nombre entier d'heures (0‑24). |
| toHours | Int32 | Heure de fin de l'intervalle représentée par un nombre entier d'heures (0‑24). |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Lorsque toTime est inférieur ou égal à l'argument toTime ou lorsque l'intervalle entre fromTime et toTime dépasse 24 heures. |

## Exemples

La surcharge du constructeur WorkingTime peut être utilisée pour initialiser le début et la fin de l'intervalle à l'aide d'heures entières :

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

Montre comment vérifier l'égalité du temps de travail.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// L'égalité des calendriers est vérifiée par rapport aux dates de début et de fin du temps de travail.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Voir aussi

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


