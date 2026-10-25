---
title: "Clase WeekDay"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.WeekDay. Representa un día de la semana que define días regulares de una semana o días de excepción en un calendario."
type: docs
weight: 3540
url: /es/net/aspose.tasks/weekday/
---
## WeekDay class

Representa un día de la semana que define días regulares de la semana o días de excepción en un calendario.

```csharp
public class WeekDay
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WeekDay](weekday/#constructor)() | Inicializa una nueva instancia de la clase `WeekDay`. |
| [WeekDay](weekday/#constructor_1)(DayType) | Inicializa una nueva instancia de la clase `WeekDay` con el tipo de día especificado. |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | Inicializa una nueva instancia de la clase `WeekDay` con el tipo de día especificado y una lista de períodos de tiempo laborables. |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | Inicializa una nueva instancia de la clase `WeekDay` con el tipo de día especificado y períodos de tiempo laborables. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Obtiene el tipo de un día. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Obtiene o establece un valor que indica si la fecha o el tipo de día especificado está laborable. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Obtiene o establece el comienzo de un tiempo de excepción. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Obtiene o establece el final de un tiempo de excepción. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Obtiene WorkingTimeCollection para esta instancia de WeekDay. La colección de tiempos laborables que define el tiempo trabajado en el día de la semana. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Crea un día laborable predeterminado. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Devuelve una copia profunda del día de la semana. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | Devuelve un valor de código hash para la instancia de la clase `WeekDay`. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Devuelve el tiempo laborable para un día de la semana. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | Convierte DayOfWeek de .Net a [`DayType`](./daytype/). |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Establece períodos de tiempo predeterminados para el día de la semana especificado. |

## Ejemplos

Muestra cómo crear un nuevo calendario definiendo los días de la semana.

```csharp
var project = new Project();

// Definir un calendar
var calendar = project.Calendars.Add("Calendar1");

// Agregar días laborables de lunes a jueves con horarios predeterminados
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// verifique las fechas de inicio y fin del día de excepción
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Establecer el viernes como día laborable corto

// Establece el tiempo laborable.
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// existe una forma de convertir <see cref=\"DayOfWeek\" /> a <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// imprimamos todos los tiempos de trabajo
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


