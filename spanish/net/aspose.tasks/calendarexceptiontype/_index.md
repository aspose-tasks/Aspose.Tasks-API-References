---
title: "Enumeración CalendarExceptionType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.CalendarExceptionType. Especifica el tipo de excepción del calendario"
type: docs
weight: 270
url: /es/net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

Especifica el tipo de excepción del calendario.

```csharp
public enum CalendarExceptionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Daily | `0` | Indica el tipo de excepción diaria. |
| YearlyByDay | `1` | Indica el tipo de excepción anual por día del mes. |
| YearlyByPosition | `2` | Indica el tipo de excepción anual por posición. |
| MonthlyByDay | `3` | Indica el tipo de excepción mensual por día del mes. |
| MonthlyByPosition | `4` | Indica el tipo de excepción mensual por posición. |
| Weekly | `5` | Indica el tipo de excepción semanal. |
| ByDayCount | `6` | Indica el tipo de excepción por recuento de días. |
| ByWeekDayCount | `7` | Indica el tipo de excepción por recuento de días de la semana. |
| NoExceptionType | `8` | Indica que no hay tipo de excepción. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


