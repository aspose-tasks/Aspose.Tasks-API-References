---
title: "CalendarException.MonthPosition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "CalendarException propiedad. Obtiene o establece la posición de un elemento de mes dentro de un mes"
type: docs
weight: 90
url: /es/net/aspose.tasks/calendarexception/monthposition/
---
## CalendarException.MonthPosition property

Obtiene o establece la posición de un elemento de mes dentro de un mes.

```csharp
public MonthPosition MonthPosition { get; set; }
```

## Ejemplos

Muestra cómo definir una excepción de calendario por día del mes.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// crear un calendario
var calendar = project.Calendars.Add("Calendar1");

// crear excepción de calendario para cada viernes
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// verificar que un viernes es excepcional
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// agrega la excepción al calendario
calendar.Exceptions.Add(exception);
```

### Ver también

* enum [MonthPosition](../../monthposition/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


