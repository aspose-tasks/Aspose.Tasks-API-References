---
title: "CalendarException.WorkingTimes"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà CalendarException. Ottiene o imposta l'oggetto WorkingTimeCollection. La collezione di tempi di lavoro che definisce il tempo lavorato nei giorni feriali. È necessario che sia presente almeno un tempo di lavoro e non possono esserci più di cinque."
type: docs
weight: 160
url: /it/net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

Ottiene o imposta l'oggetto WorkingTimeCollection. La collezione di orari di lavoro che definisce il tempo lavorato nei giorni feriali. Deve essere presente almeno un orario di lavoro e non possono esserne più di cinque.

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

## Esempi

Mostra come ottenere il tempo di lavoro di un'eccezione di calendario.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];
var exception = calendar.Exceptions[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
Console.WriteLine("Calendar Exception Name: " + exception.Name);
Console.WriteLine();

var workingTime = exception.GetWorkingTime();
Console.WriteLine("Exception Working Time: " + workingTime);

foreach (var time in exception.WorkingTimes)
{
    Console.WriteLine("Working Time Start: " + time.From);
    Console.WriteLine("Working Time Finish: " + time.To);
}
```

### Vedi anche

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


