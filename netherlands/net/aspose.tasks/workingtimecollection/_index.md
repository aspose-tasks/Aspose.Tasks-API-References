---
title: "Klasse WorkingTimeCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WorkingTimeCollection klasse. Vertegenwoordigt een verzameling van WorkingTimeCollection‑objecten."
type: docs
weight: 3670
url: /nl/net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

Vertegenwoordigt een verzameling van `WorkingTimeCollection` objecten.

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | Haalt het aantal objecten op dat in dit `WorkingTimeCollection` object is opgenomen. |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | Retourneert het element op de opgegeven index. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | Voegt een nieuw WorkingTime‑exemplaar toe aan deze verzameling. |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | Verwijdert alle [`WorkingTime`](../workingtime/) items uit de verzameling. |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | Controleert of het opgegeven element in de lijst staat. Voert een lineaire O(n)‑zoekactie uit. |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | Kopieert de inhoud van een verzameling naar een Array, beginnend op een bepaalde index. |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | Verwijdert een [`WorkingTime`](../workingtime/) exemplaar uit deze verzameling. |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | Converteert het WorkingTimeCollection‑object naar een lijst van [`WorkingTime`](../workingtime/) objecten. |

## Voorbeelden

Toont hoe te werken met een working time‑verzameling.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// print werktijden van zaterdag
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// print werktijden van zondag
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // Je kunt verder door werktijden navigeren en deze weergeven
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### Zie ook

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


