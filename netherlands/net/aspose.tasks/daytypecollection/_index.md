---
title: "Klasse DayTypeCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.DayTypeCollection klasse. Vertegenwoordigt een collectie van DayType-objecten"
type: docs
weight: 460
url: /nl/net/aspose.tasks/daytypecollection/
---
## DayTypeCollection class

Vertegenwoordigt een collectie van [`DayType`](../daytype/) objecten.

```csharp
public class DayTypeCollection : IList<DayType>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/daytypecollection/count/) { get; } | Haalt het aantal elementen op dat in deze collectie zit. |
| [IsReadOnly](../../aspose.tasks/daytypecollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders false. |
| [Item](../../aspose.tasks/daytypecollection/item/) { get; set; } | Retourneert of stelt het element in op de opgegeven index. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/daytypecollection/add/)(DayType) | Voegt het opgegeven item toe aan deze collectie. |
| [Clear](../../aspose.tasks/daytypecollection/clear/)() | Verwijdert alle items uit deze collectie. |
| [Contains](../../aspose.tasks/daytypecollection/contains/)(DayType) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [CopyTo](../../aspose.tasks/daytypecollection/copyto/)(DayType[], int) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [GetEnumerator](../../aspose.tasks/daytypecollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [IndexOf](../../aspose.tasks/daytypecollection/indexof/)(DayType) | Bepaalt de index van het opgegeven item in deze collectie. |
| [Insert](../../aspose.tasks/daytypecollection/insert/)(int, DayType) | Voegt het opgegeven item in op de opgegeven index. |
| [Remove](../../aspose.tasks/daytypecollection/remove/)(DayType) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |
| [RemoveAt](../../aspose.tasks/daytypecollection/removeat/)(int) | Verwijdert een item op de opgegeven index. |

## Voorbeelden

Toont hoe een weekdagencollectie te gebruiken om een wekelijkse kalenderuitzondering te definiëren.

```csharp
var project = new Project(DataDir + "WeeklyDayTypeException.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Exception Name: " + calendarException.Name);
    Console.WriteLine("Days of week count: " + calendarException.DaysOfWeek.Count);
    foreach (var dayType in calendarException.DaysOfWeek)
    {
        Console.WriteLine("Day type: " + dayType);
    }

    Console.WriteLine();
}

var exc1 = calendar.Exceptions.ToList()[0];
if (!exc1.DaysOfWeek.IsReadOnly && exc1.DaysOfWeek.IndexOf(DayType.Monday) < 0)
{
    exc1.DaysOfWeek.Insert(0, DayType.Wednesday);
}

var exc2 = calendar.Exceptions.ToList()[1];
if (exc2.DaysOfWeek.Contains(DayType.Sunday))
{
    // verwijder een dagtype uit "Exception 2" op basis van dagtype
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// verwijder een dagtype uit "Exception 2" op basis van index
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// Wijzig uitzonderingen (er zijn geen uitzonderingen in de initiële projectgegevens)
var exc4 = new CalendarException
               {
                   Name = "Weekly Exception 2",
                   FromDate = new DateTime(2020, 4, 13),
                   ToDate = new DateTime(2020, 4, 18),
                   Occurrences = 3,
                   Type = CalendarExceptionType.Weekly
               };
exc4.DaysOfWeek.Add(DayType.Monday);
exc4.DaysOfWeek.Add(DayType.Thursday);

calendar.Exceptions.Add(exc4);

var exc3 = calendar.Exceptions.ToList()[2];

// verwijder alle weekdagen voor "Exception 3"
exc3.DaysOfWeek.Clear();

var dayTypes = new DayType[exc4.DaysOfWeek.Count];
exc4.DaysOfWeek.CopyTo(dayTypes, 0);

foreach (var dayType in dayTypes)
{
    exc3.DaysOfWeek.Add(dayType);
}

Console.WriteLine("Days of week for exception: " + exc3.Name);
foreach (var dayType in exc3.DaysOfWeek)
{
    Console.WriteLine("Day type: " + dayType);
}
```

### Zie ook

* enum [DayType](../daytype/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


