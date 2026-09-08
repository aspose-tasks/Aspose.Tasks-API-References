---
title: "CalendarException.Period"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "CalendarException propiedad. Obtiene o establece el período de recurrencia para la excepción."
type: docs
weight: 130
url: /es/net/aspose.tasks/calendarexception/period/
---
## CalendarException.Period property

Obtiene o establece el período de recurrencia de la excepción.

```csharp
public int Period { get; set; }
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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


