---
title: "CalendarException.GetWorkingTime"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo CalendarException. Restituisce il tempo di lavoro per un'eccezione di calendario."
type: docs
weight: 200
url: /it/net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

Restituisce il tempo di lavoro per un'eccezione del calendario.

```csharp
public TimeSpan GetWorkingTime()
```

### Valore di ritorno

Restituisce il tempo di lavoro per questa eccezione di calendario.

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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


