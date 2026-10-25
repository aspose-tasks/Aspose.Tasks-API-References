---
title: "Enum MonthItemType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enum Aspose.Tasks.MonthItemType. Especifica el elemento de mes para el cual se programa una recurrencia de excepción."
type: docs
weight: 1050
url: /es/net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

Especifica el elemento del mes para el cual se programa una recurrencia de excepción.

```csharp
public enum MonthItemType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | Indica tipo de elemento de mes indefinido. |
| Day | `0` | Indica tipo de elemento de mes día. |
| Weekday | `1` | Indica tipo de elemento de mes día laborable. |
| WeekendDay | `2` | Indica tipo de elemento de mes día de fin de semana. |
| Sunday | `3` | Indica tipo de elemento de mes domingo. |
| Monday | `4` | Indica tipo de elemento de mes lunes. |
| Tuesday | `5` | Indica tipo de elemento de mes martes. |
| Wednesday | `6` | Indica tipo de elemento de mes miércoles. |
| Thursday | `7` | Indica tipo de elemento de mes jueves. |
| Friday | `8` | Indica tipo de elemento de mes viernes. |
| Saturday | `9` | Indica tipo de elemento de mes sábado. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


