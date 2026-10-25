---
title: "CalendarException.Delete"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "CalendarException metodo. Elimina l'istanza Exception dal calendario genitore oggetto CalendarExceptionCollection"
type: docs
weight: 180
url: /it/net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

Elimina l'istanza Exception dall'oggetto CalendarExceptionCollection del calendario padre.

```csharp
public void Delete()
```

## Esempi

Mostra come eliminare un'eccezione di calendario.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// rimuovi l'eccezione
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### Vedi anche

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


