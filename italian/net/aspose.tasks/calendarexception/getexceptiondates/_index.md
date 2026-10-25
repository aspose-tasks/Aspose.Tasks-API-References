---
title: "CalendarException.GetExceptionDates"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "CalendarException metodo. Restituisce le date in cui l'eccezione del calendario è applicabile"
type: docs
weight: 190
url: /it/net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

Restituisce le date in cui l'eccezione del calendario è applicabile.

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### Valore di ritorno

Restituisce una collezione di date di eccezione per le quali l'eccezione del calendario è applicabile.

## Esempi

Mostra come ottenere le date per le quali una specifica eccezione del calendario è efficace.

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### Vedi anche

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


