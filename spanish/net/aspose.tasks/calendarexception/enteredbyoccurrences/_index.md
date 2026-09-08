---
title: "CalendarException.EnteredByOccurrences"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "CalendarException propiedad. Obtiene o establece un valor que indica si el rango de recurrencia se define ingresando un número de ocurrencias. False especifica que el rango de recurrencia se define ingresando una fecha de finalización."
type: docs
weight: 40
url: /es/net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

Obtiene o establece un valor que indica si el rango de recurrencia se define ingresando un número de ocurrencias. False especifica que el rango de recurrencia se define ingresando una fecha de finalización.

```csharp
public bool EnteredByOccurrences { get; set; }
```

## Ejemplos

Muestra cómo definir una excepción de calendario por ocurrencias.

```csharp
var project = new Project();

// Definir un calendar
var calendar = project.Calendars.Add("Calendar1");

// Definir excepción y especificar ocurrencias
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// Agregar excepción al calendario
calendar.Exceptions.Add(exception);
```

### Ver también

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


