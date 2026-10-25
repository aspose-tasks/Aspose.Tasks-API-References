---
title: "Clase CalendarException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.CalendarException. Representa períodos de tiempo excepcionales en un calendario"
type: docs
weight: 250
url: /es/net/aspose.tasks/calendarexception/
---
## CalendarException class

Representa períodos de tiempo excepcionales en un calendario.

```csharp
public sealed class CalendarException
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CalendarException](calendarexception/)() | Inicializa una nueva instancia de la clase `CalendarException`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | Obtiene la DayTypeCollection para este objecto. Los días de la semana en los que la excepción es válida. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | Obtiene o establece un valor que indica si la fecha o el tipo de día especificado está laborable. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | Obtiene o establece un valor que indica si el rango de recurrencia se define ingresando un número de ocurrencias. False especifica que el rango de recurrencia se define ingresando una fecha de finalización. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | Obtiene o establece el comienzo del tiempo de la excepción. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | Obtiene o establece el mes para el cual se programa una recurrencia de excepción. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | Obtiene o establece el día del mes en el que se programa una recurrencia de excepción. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | Obtiene o establece el elemento de mes para el cual se programa una recurrencia de excepción. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | Obtiene o establece la posición de un elemento de mes dentro de un mes. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | Obtiene o establece el nombre de la excepción. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | Obtiene o establece el número de ocurrencias para las que la excepción del calendario es válida. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | Obtiene el calendario principal para este objeto. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | Obtiene o establece el período de recurrencia de la excepción. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | Obtiene o establece el final del tiempo de la excepción. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | Obtiene o establece el tipo de excepción. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | Obtiene o establece el objeto WorkingTimeCollection. La colección de tiempos de trabajo que define el tiempo trabajado en el día laborable. Al menos un tiempo de trabajo debe estar presente, y no puede haber más de cinco. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | Devuelve true si la instancia especificada de la estructura DateTime es el día de excepción. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | Elimina la instancia Exception del objeto CalendarExceptionCollection del calendario principal. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | Devuelve las fechas en las que la excepción del calendario es aplicable. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | Devuelve el tiempo de trabajo para una excepción del calendario. |

## Ejemplos

Muestra cómo agregar/eliminar excepciones del calendario.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// crear un calendario
var calendar = project.Calendars.Add("Calendar1");

// crear excepción de días de la semana para un día festivo
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// verificar que la fecha sea excepcional
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// eliminar una excepción
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// agregar una excepción
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// imprimir excepciones
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


