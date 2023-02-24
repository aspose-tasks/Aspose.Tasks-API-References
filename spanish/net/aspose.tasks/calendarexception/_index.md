---
title: Class CalendarException
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Aspose.Tasks.CalendarException clase. Representar periodos de tiempo excepcionales en un calendario.
type: docs
weight: 250
url: /es/net/aspose.tasks/calendarexception/
---
## CalendarException class

Representar periodos de tiempo excepcionales en un calendario.

```csharp
public sealed class CalendarException
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CalendarException](calendarexception/)() | Inicializa una nueva instancia del`CalendarException` clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | Obtiene DayTypeCollection para este objeto. Los días de la semana en los que la excepción es válida. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | Obtiene o establece un valor que indica si la fecha o el tipo de día especificado está funcionando. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | Obtiene o establece un valor que indica si el rango de recurrencia se define ingresando un número de ocurrencias. False especifica que el rango de recurrencia se define ingresando una fecha de finalización. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | Obtiene o establece el inicio del tiempo de excepción. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | Obtiene o establece el mes para el que se programa una recurrencia de excepción. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | Obtiene o establece el día de un mes en el que está programada la recurrencia de una excepción. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | Obtiene o establece el elemento del mes para el que está programada una recurrencia de excepción. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | Obtiene o establece la posición de un elemento de mes dentro de un mes. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | Obtiene o establece el nombre de la excepción. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | Obtiene o establece el número de ocurrencias para las que la excepción de calendario es válida. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | Obtiene el calendario principal para este objeto. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | Obtiene o establece el período de recurrencia de la excepción. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | Obtiene o establece el final del tiempo de excepción. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | Obtiene o establece el tipo de excepción. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | Obtiene o establece el objeto WorkingTimeCollection. La colección de tiempos de trabajo que define el tiempo trabajado en el día de la semana.  Debe presentarse al menos un horario de trabajo, y no pueden ser más de cinco. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | Devuelve verdadero si la instancia especificada delDateTime struct es la excepción día. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | Elimina la instancia de excepción del objeto CalendarExceptionCollection del calendario principal. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | Devuelve las fechas en las que se aplica la excepción del calendario. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | Devuelve el tiempo de trabajo para una excepción de calendario. |

### Ver también

* espacio de nombres [Aspose.Tasks](../../aspose.tasks/)
* asamblea [Aspose.Tasks](../../)


