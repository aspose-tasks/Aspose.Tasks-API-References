---
title: "CalendarException.FromDate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarException property. Haalt het begin van de uitzonderingstijd op of stelt deze in."
type: docs
weight: 50
url: /nl/net/aspose.tasks/calendarexception/fromdate/
---
## CalendarException.FromDate property

Haalt op of stelt het begin van de uitzonderingstijd in.

```csharp
public DateTime FromDate { get; set; }
```

## Voorbeelden

Toont hoe u kalenderuitzonderingen kunt toevoegen/verwijderen.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// maak een kalender
var calendar = project.Calendars.Add("Calendar1");

// maak een weekdagenuitzondering voor een feestdag
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// controleer of de datum uitzonderlijk is
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// verwijder een uitzondering
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// voeg een uitzondering toe
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// print uitzonderingen
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### Zie ook

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


