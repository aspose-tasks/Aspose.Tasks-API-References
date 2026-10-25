---
title: "CalendarException.CalendarException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "CalendarException constructor. Inicializa una nueva instancia de la clase CalendarException."
type: docs
weight: 10
url: /es/net/aspose.tasks/calendarexception/calendarexception/
---
## CalendarException constructor

Inicializa una nueva instancia de la clase [`CalendarException`](../).

```csharp
public CalendarException()
```

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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


