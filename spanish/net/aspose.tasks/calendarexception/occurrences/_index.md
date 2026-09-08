---
title: "CalendarException.Occurrences"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "CalendarException propiedad. Obtiene o establece el número de ocurrencias para las que la excepción de calendario es válida"
type: docs
weight: 110
url: /es/net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

Obtiene o establece el número de ocurrencias para las que la excepción del calendario es válida.

```csharp
public int Occurrences { get; set; }
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


