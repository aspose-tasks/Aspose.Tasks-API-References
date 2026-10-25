---
title: "WorkingTime.WorkingTime"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "WorkingTime constructor. Initialiseert een nieuw exemplaar van de WorkingTime-klasse met een interval met de opgegeven start- en eindtijden"
type: docs
weight: 10
url: /nl/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`WorkingTime`](../) klasse met een interval met de opgegeven start- en eindtijden.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fromTime | DateTime | interval starttijd |
| toTime | DateTime | interval eindtijd |

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

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`WorkingTime`](../) klasse met een interval-item met de opgegeven start- en eindtijden.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fromTime | TimeSpan | Starttijd van het interval wordt weergegeven door de TimeSpan-struct. |
| toTime | TimeSpan | Eindtijd van het interval wordt weergegeven door de TimeSpan-struct. |

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentException | Wanneer toTime kleiner is dan of gelijk aan toTime-argument of wanneer het interval tussen fromTime en toTime groter is dan 24 uur. |

## Voorbeelden

De overload van WorkingTime ctor kan worden gebruikt om het begin en einde van het interval te initialiseren met TimeSpans:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### Zie ook

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Initialiseert een nieuw exemplaar van de [`WorkingTime`](../) klasse met een interval-item met de opgegeven start- en eindtijden.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fromHours | Int32 | De starttijd van het interval wordt weergegeven door een geheel aantal uren (0-24). |
| toHours | Int32 | De eindtijd van het interval wordt weergegeven door een geheel aantal uren (0-24). |

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentException | Wanneer toTime kleiner is dan of gelijk aan toTime-argument of wanneer het interval tussen fromTime en toTime groter is dan 24 uur. |

## Voorbeelden

De overload van WorkingTime ctor kan worden gebruikt om het begin en einde van het interval te initialiseren met hele uren:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

Toont hoe de gelijkheid van werktijd te controleren.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// De gelijkheid van kalenders wordt gecontroleerd aan de hand van de van- en tot-datums van de werktijd.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Zie ook

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


