---
title: "CalendarException.WorkingTimes"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "CalendarException propiedad. Obtiene o establece el objeto WorkingTimeCollection. La colección de tiempos de trabajo que define el tiempo trabajado en el día laborable. Al menos un tiempo de trabajo debe estar presente y no puede haber más de cinco."
type: docs
weight: 160
url: /es/net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

Obtiene o establece el objeto WorkingTimeCollection. La colección de tiempos de trabajo que define el tiempo trabajado en el día laborable. Al menos un tiempo de trabajo debe estar presente, y no puede haber más de cinco.

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


