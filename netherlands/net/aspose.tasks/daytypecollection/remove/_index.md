---
title: "DayTypeCollection.Remove"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "DayTypeCollection methode. Verwijdert de eerste instantie van een specifiek object uit deze collectie"
type: docs
weight: 110
url: /nl/net/aspose.tasks/daytypecollection/remove/
---
## DayTypeCollection.Remove method

Verwijdert de eerste instantie van een specifiek object uit deze collectie.

```csharp
public bool Remove(DayType item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | DayType | het opgegeven object om te verwijderen. |

### Retourwaarde

true als het opgegeven object succesvol uit deze collectie is verwijderd; anders false.

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

* enum [DayType](../../daytype/)
* class [DayTypeCollection](../)
* namespace [Aspose.Tasks](../../daytypecollection/)
* assembly [Aspose.Tasks](../../../)


