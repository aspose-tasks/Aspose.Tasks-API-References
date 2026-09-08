---
title: "Enumeración MonthPosition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.MonthPosition enum. Especifica la posición de un elemento de mes dentro de un mes."
type: docs
weight: 1070
url: /es/net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

Especifica la posición de un elemento del mes dentro de un mes.

```csharp
public enum MonthPosition
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | Indica posición de mes indefinida. |
| First | `0` | Indica la primera posición del mes. |
| Second | `1` | Indica la segunda posición del mes. |
| Third | `2` | Indica la tercera posición del mes. |
| Fourth | `3` | Indica la posición del cuarto mes. |
| Last | `4` | Indica la posición del último mes. |

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


