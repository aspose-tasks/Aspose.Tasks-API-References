---
title: "Clase WeekDayCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.WeekDayCollection. Representa una colección de objetos WeekDay"
type: docs
weight: 3550
url: /es/net/aspose.tasks/weekdaycollection/
---
## WeekDayCollection class

Representa una colección de objetos [`WeekDay`](../weekday/).

```csharp
public class WeekDayCollection : IList<WeekDay>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/weekdaycollection/count/) { get; } | Obtiene el número de objetos contenidos en este objeto `WeekDayCollection`. |
| [Item](../../aspose.tasks/weekdaycollection/item/) { get; set; } | Obtiene o establece el valor del elemento en el índice especificado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/weekdaycollection/add/)(WeekDay) | Agrega una instancia de [`WeekDay`](../weekday/) a este objeto. |
| [Clear](../../aspose.tasks/weekdaycollection/clear/)() | Limpia el objeto WeekDayCollection. |
| [Contains](../../aspose.tasks/weekdaycollection/contains/)(WeekDay) | Comprueba si la colección contiene el [`WeekDay`](../weekday/) especificado. |
| [CopyTo](../../aspose.tasks/weekdaycollection/copyto/)(WeekDay[], int) | Copia el contenido de la colección a una matriz en el índice especificado. |
| [GetEnumerator](../../aspose.tasks/weekdaycollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [IndexOf](../../aspose.tasks/weekdaycollection/indexof/)(WeekDay) | Devuelve el índice del [`WeekDay`](../weekday/) especificado. |
| [Insert](../../aspose.tasks/weekdaycollection/insert/)(int, WeekDay) | Inserta el [`WeekDay`](../weekday/) en el índice especificado. |
| [Remove](../../aspose.tasks/weekdaycollection/remove/)(WeekDay) | Elimina el [`WeekDay`](../weekday/) especificado, si existe. |
| [RemoveAt](../../aspose.tasks/weekdaycollection/removeat/)(int) | Elimina un elemento en el índice especificado. |
| [ToList](../../aspose.tasks/weekdaycollection/tolist/)() | Convierte el objeto WeekDayCollection en una lista de objetos [`WeekDay`](../weekday/). |

## Ejemplos

Muestra cómo trabajar con colecciones de días de la semana.

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// limpiar días de la semana
calendar.WeekDays.Clear();

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
var saturday = WeekDay.CreateDefaultWorkingDay(DayType.Saturday);
var sunday = WeekDay.CreateDefaultWorkingDay(DayType.Sunday);

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

var fridayWorkingTimes = new List<WorkingTime> { new WorkingTime(new DateTime(2020, 4, 13, 8, 0, 0), new DateTime(2020, 4, 13, 12, 0, 0)) };

var friday = new WeekDay(DayType.Friday, fridayWorkingTimes);
if (calendar.WeekDays.Contains(friday))
{
    calendar.WeekDays.Insert(4, friday);
}

Console.WriteLine("Calendar: " + calendar.Name);
Console.WriteLine("Week days count: " + calendar.WeekDays.Count);
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

// eliminar sábado día de la semana
calendar.WeekDays.RemoveAt(5);

// eliminar domingo día de la semana
if (calendar.WeekDays.IndexOf(saturday) > 0)
{
    calendar.WeekDays.Remove(sunday);
}

Console.WriteLine("Working times after weekend was removed: ");
List<WeekDay> weekDays = calendar.WeekDays.ToList();
foreach (var day in weekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

var hour24Calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(hour24Calendar);

// copiar días de la semana
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### Ver también

* class [WeekDay](../weekday/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


