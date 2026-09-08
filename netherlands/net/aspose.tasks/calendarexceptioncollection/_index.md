---
title: "Klasse CalendarExceptionCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.CalendarExceptionCollection klasse. Vertegenwoordigt een collectie van CalendarException-objecten"
type: docs
weight: 260
url: /nl/net/aspose.tasks/calendarexceptioncollection/
---
## CalendarExceptionCollection class

Vertegenwoordigt een collectie van [`CalendarException`](../calendarexception/) objecten.

```csharp
public class CalendarExceptionCollection : IList<CalendarException>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/calendarexceptioncollection/count/) { get; } | Haalt het aantal objecten op dat in dit `CalendarExceptionCollection`-object zit. |
| [Item](../../aspose.tasks/calendarexceptioncollection/item/) { get; set; } | Retourneert het element op de opgegeven index. |
| [ParentCalendar](../../aspose.tasks/calendarexceptioncollection/parentcalendar/) { get; } | Haalt de bovenliggende agenda op voor dit object. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/calendarexceptioncollection/add/)(CalendarException) | Voegt een CalendarException‑instantie toe aan dit collectie‑object. |
| [AddRange](../../aspose.tasks/calendarexceptioncollection/addrange/)(IEnumerable&lt;CalendarException&gt;) | Voegt een reeks uitzonderingen toe aan de interne lijst. |
| [Clear](../../aspose.tasks/calendarexceptioncollection/clear/)() | Verwijdert alle items uit de `CalendarExceptionCollection`. |
| [GetEnumerator](../../aspose.tasks/calendarexceptioncollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/calendarexceptioncollection/remove/)(CalendarException) | Verwijdert een [`CalendarException`](../calendarexception/)‑instantie uit deze collectie. |
| [ToList](../../aspose.tasks/calendarexceptioncollection/tolist/)() | Converteert het CalendarExceptionCollection‑object naar een lijst van [`CalendarException`](../calendarexception/) objecten. |

## Voorbeelden

Toont hoe de calendar exception‑collectie te gebruiken om kalenderuitzonderingen te definiëren.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByUid(3);

calendar.Exceptions.Clear();
Calendar.MakeStandardCalendar(calendar);

var exception = new CalendarException();
exception.FromDate = new DateTime(2020, 3, 30, 8, 0, 0);
exception.ToDate = new DateTime(2020, 4, 3, 17, 0, 0);
exception.DayWorking = true;
exception.Name = "Exception 1";

var wt1 = new WorkingTime(9, 13);
var wt2 = new WorkingTime(14, 19);

exception.WorkingTimes.Add(wt1);
exception.WorkingTimes.Add(wt2);
calendar.Exceptions.Add(exception);

var nonWorkingExceptions = new CalendarException[2];
nonWorkingExceptions[0] = new CalendarException();
nonWorkingExceptions[0].FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
nonWorkingExceptions[0].ToDate = new DateTime(2020, 4, 18, 17, 0, 0);
nonWorkingExceptions[0].DayWorking = false;
nonWorkingExceptions[0].Name = "Exception 2";
nonWorkingExceptions[1] = new CalendarException();
nonWorkingExceptions[1].FromDate = new DateTime(2020, 4, 6, 8, 0, 0);
nonWorkingExceptions[1].ToDate = new DateTime(2020, 4, 10, 17, 0, 0);
nonWorkingExceptions[1].DayWorking = false;
nonWorkingExceptions[1].Name = "Exception 3";
calendar.Exceptions.AddRange(nonWorkingExceptions);

Console.WriteLine("Exceptions of calendar {0}: ", calendar.Exceptions.ParentCalendar.Name);
Console.WriteLine("Exceptions count: {0}", calendar.Exceptions.Count);
Console.WriteLine();
foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Name: " + calendarException.Name);
    Console.WriteLine("From Date: " + calendarException.FromDate);
    Console.WriteLine("To Date: " + calendarException.ToDate);
    Console.WriteLine("Is day working: " + calendarException.DayWorking);
    Console.WriteLine();
}

// verwijder alle uitzonderingen
Console.WriteLine("Remove calendar exceptions...");
List<CalendarException> exceptions = calendar.Exceptions.ToList();
foreach (var calendarException in exceptions)
{
    Console.WriteLine("Remove exception: " + calendarException.Name);
    Console.WriteLine();
    calendar.Exceptions.Remove(calendarException);
}
```

### Zie ook

* class [CalendarException](../calendarexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


