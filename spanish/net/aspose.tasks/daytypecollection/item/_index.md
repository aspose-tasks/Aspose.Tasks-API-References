---
title: "DayTypeCollection.Item"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad DayTypeCollection. Obtiene o establece el elemento en el índice especificado"
type: docs
weight: 30
url: /es/net/aspose.tasks/daytypecollection/item/
---
## DayTypeCollection indexer

Devuelve o establece el elemento en el índice especificado.

```csharp
public DayType this[int index] { get; set; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento a obtener o establecer. |

### Valor devuelto

el elemento en el índice especificado.

## Ejemplos

Muestra cómo usar una colección de días de la semana para definir una excepción de calendario semanal.

```csharp
var project = new Project(DataDir + "WeeklyDayTypeException.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Exception Name: " + calendarException.Name);
    Console.WriteLine("Days of week count: " + calendarException.DaysOfWeek.Count);
    foreach (var dayType in calendarException.DaysOfWeek)
    {
        Console.WriteLine("Day type: " + dayType);
    }

    Console.WriteLine();
}

var exc1 = calendar.Exceptions.ToList()[0];
if (!exc1.DaysOfWeek.IsReadOnly && exc1.DaysOfWeek.IndexOf(DayType.Monday) < 0)
{
    exc1.DaysOfWeek.Insert(0, DayType.Wednesday);
}

var exc2 = calendar.Exceptions.ToList()[1];
if (exc2.DaysOfWeek.Contains(DayType.Sunday))
{
    // eliminar un tipo de día de "Exception 2" por tipo de día
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// eliminar un tipo de día de "Exception 2" por índice
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// Cambiar excepciones (no hay excepciones en los datos iniciales del proyecto)
var exc4 = new CalendarException
               {
                   Name = "Weekly Exception 2",
                   FromDate = new DateTime(2020, 4, 13),
                   ToDate = new DateTime(2020, 4, 18),
                   Occurrences = 3,
                   Type = CalendarExceptionType.Weekly
               };
exc4.DaysOfWeek.Add(DayType.Monday);
exc4.DaysOfWeek.Add(DayType.Thursday);

calendar.Exceptions.Add(exc4);

var exc3 = calendar.Exceptions.ToList()[2];

// eliminar todos los días de la semana para "Exception 3"
exc3.DaysOfWeek.Clear();

var dayTypes = new DayType[exc4.DaysOfWeek.Count];
exc4.DaysOfWeek.CopyTo(dayTypes, 0);

foreach (var dayType in dayTypes)
{
    exc3.DaysOfWeek.Add(dayType);
}

Console.WriteLine("Days of week for exception: " + exc3.Name);
foreach (var dayType in exc3.DaysOfWeek)
{
    Console.WriteLine("Day type: " + dayType);
}
```

### Ver también

* enum [DayType](../../daytype/)
* class [DayTypeCollection](../)
* namespace [Aspose.Tasks](../../daytypecollection/)
* assembly [Aspose.Tasks](../../../)


