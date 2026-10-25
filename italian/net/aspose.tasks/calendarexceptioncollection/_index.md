---
title: "Classe CalendarExceptionCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.CalendarExceptionCollection classe. Rappresenta una raccolta di oggetti CalendarException"
type: docs
weight: 260
url: /it/net/aspose.tasks/calendarexceptioncollection/
---
## CalendarExceptionCollection class

Rappresenta una raccolta di [`CalendarException`](../calendarexception/) oggetti.

```csharp
public class CalendarExceptionCollection : IList<CalendarException>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/calendarexceptioncollection/count/) { get; } | Ottiene il numero di oggetti contenuti in questo oggetto `CalendarExceptionCollection`. |
| [Item](../../aspose.tasks/calendarexceptioncollection/item/) { get; set; } | Restituisce l'elemento all'indice specificato. |
| [ParentCalendar](../../aspose.tasks/calendarexceptioncollection/parentcalendar/) { get; } | Ottiene il calendario principale per questo oggetto. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/calendarexceptioncollection/add/)(CalendarException) | Aggiunge l'istanza CalendarException a questo oggetto di raccolta. |
| [AddRange](../../aspose.tasks/calendarexceptioncollection/addrange/)(IEnumerable&lt;CalendarException&gt;) | Aggiunge un intervallo di eccezioni all'elenco interno. |
| [Clear](../../aspose.tasks/calendarexceptioncollection/clear/)() | Rimuove tutti gli elementi da `CalendarExceptionCollection`. |
| [GetEnumerator](../../aspose.tasks/calendarexceptioncollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/calendarexceptioncollection/remove/)(CalendarException) | Rimuove l'istanza [`CalendarException`](../calendarexception/) da questa raccolta. |
| [ToList](../../aspose.tasks/calendarexceptioncollection/tolist/)() | Converte l'oggetto CalendarExceptionCollection in un elenco di oggetti [`CalendarException`](../calendarexception/). |

## Esempi

Mostra come utilizzare la raccolta di eccezioni del calendario per definire le eccezioni del calendario.

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

// rimuovi tutte le eccezioni
Console.WriteLine("Remove calendar exceptions...");
List<CalendarException> exceptions = calendar.Exceptions.ToList();
foreach (var calendarException in exceptions)
{
    Console.WriteLine("Remove exception: " + calendarException.Name);
    Console.WriteLine();
    calendar.Exceptions.Remove(calendarException);
}
```

### Vedi anche

* class [CalendarException](../calendarexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


