---
title: "CalendarException.Delete"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "CalendarException método. Elimina la instancia Exception del objeto CalendarExceptionCollection del calendario padre"
type: docs
weight: 180
url: /es/net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

Elimina la instancia Exception del objeto CalendarExceptionCollection del calendario principal.

```csharp
public void Delete()
```

## Ejemplos

Muestra cómo eliminar una excepción de calendario.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// eliminar la excepción
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### Ver también

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


