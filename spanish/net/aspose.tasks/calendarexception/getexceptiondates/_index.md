---
title: "CalendarException.GetExceptionDates"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método CalendarException. Devuelve las fechas en las que la excepción del calendario es aplicable"
type: docs
weight: 190
url: /es/net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

Devuelve las fechas en las que la excepción del calendario es aplicable.

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### Valor devuelto

Devuelve una colección de fechas de excepción para las que la excepción del calendario es aplicable.

## Ejemplos

Muestra cómo obtener las fechas para las que una excepción de calendario específica es efectiva.

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### Ver también

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


