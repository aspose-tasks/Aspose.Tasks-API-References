---
title: "CalendarException.GetWorkingTime"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "CalendarException método. Devuelve el tiempo de trabajo para una excepción de calendario."
type: docs
weight: 200
url: /es/net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

Devuelve el tiempo de trabajo para una excepción del calendario.

```csharp
public TimeSpan GetWorkingTime()
```

### Valor devuelto

Devuelve el tiempo de trabajo para esta excepción de calendario.

## Ejemplos

Muestra cómo obtener el tiempo de trabajo de una excepción de calendario.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];
var exception = calendar.Exceptions[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
Console.WriteLine("Calendar Exception Name: " + exception.Name);
Console.WriteLine();

var workingTime = exception.GetWorkingTime();
Console.WriteLine("Exception Working Time: " + workingTime);

foreach (var time in exception.WorkingTimes)
{
    Console.WriteLine("Working Time Start: " + time.From);
    Console.WriteLine("Working Time Finish: " + time.To);
}
```

### Ver también

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


