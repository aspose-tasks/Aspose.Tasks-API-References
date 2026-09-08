---
title: "Klasse CalendarException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.CalendarException klasse. Vertegenwoordigt uitzonderlijke tijdsperioden in een kalender"
type: docs
weight: 250
url: /nl/net/aspose.tasks/calendarexception/
---
## CalendarException class

Stelt uitzonderlijke tijdsperioden in een kalender voor.

```csharp
public sealed class CalendarException
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [CalendarException](calendarexception/)() | Initialiseert een nieuw exemplaar van de `CalendarException` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | Haalt de DayTypeCollection op voor dit object. De dagen van de week waarop de uitzondering geldig is. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of de opgegeven datum of het dagtype een werkdag is. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of het bereik van herhaling wordt gedefinieerd door een aantal herhalingen in te voeren. False geeft aan dat het bereik van herhaling wordt gedefinieerd door een einddatum in te voeren. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | Haalt op of stelt het begin van de uitzonderingstijd in. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | Haalt op of stelt de maand in waarvoor een uitzonderingherhaling is gepland. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | Haalt op of stelt de dag van de maand in waarop een uitzonderingherhaling is gepland. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | Haalt op of stelt het maandelement in waarvoor een uitzonderingherhaling is gepland. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | Haalt op of stelt de positie van een maandelement binnen een maand in. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | Haalt op of stelt de naam van de uitzondering in. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | Haalt op of stelt het aantal herhalingen in waarvoor de kalenderuitzondering geldig is. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | Haalt de bovenliggende agenda op voor dit object. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | Haalt op of stelt de periode van herhaling voor de uitzondering in. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | Haalt op of stelt het einde van de uitzonderingstijd in. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | Haalt op of stelt het type van de uitzondering in. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | Haalt op of stelt het WorkingTimeCollection-object in. De collectie werktijden die de gewerkte tijd op een weekdag definieert. Er moet minstens één werktijd aanwezig zijn, en er kunnen niet meer dan vijf zijn. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | Retourneert true als de opgegeven instantie van de DateTime-structuur de uitzonderingsdag is. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | Verwijdert de Exception-instantie uit het bovenliggende kalenderobject CalendarExceptionCollection. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | Retourneert data waarop de kalenderuitzondering van toepassing is. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | Retourneert de werktijd voor een kalenderuitzondering. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


