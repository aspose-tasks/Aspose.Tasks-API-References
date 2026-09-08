---
title: "CalendarException.DaysOfWeek"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "CalendarException propiedad. Obtiene la DayTypeCollection para este objeto. Los días de la semana en los que la excepción es válida"
type: docs
weight: 20
url: /es/net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

Obtiene la DayTypeCollection para este objecto. Los días de la semana en los que la excepción es válida.

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## Ejemplos

Muestra cómo definir una excepción de calendario por día de la semana.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// crear un calendario
var calendar = project.Calendars.Add("Calendar1");

// crear excepción de calendario para cada viernes
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// verifica que el viernes sea excepcional
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// agrega la excepción al calendario
calendar.Exceptions.Add(exception);
```

### Ver también

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


