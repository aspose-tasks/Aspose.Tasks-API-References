---
title: "CalendarException.MonthDay"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "CalendarException propiedad. Obtiene o establece el día del mes en el que se programa una recurrencia de excepción"
type: docs
weight: 70
url: /es/net/aspose.tasks/calendarexception/monthday/
---
## CalendarException.MonthDay property

Obtiene o establece el día del mes en el que se programa una recurrencia de excepción.

```csharp
public int MonthDay { get; set; }
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


