---
title: "WeekDay.SetDefaultWorkingTime"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método WeekDay. Establece los períodos de tiempo predeterminados para el día de la semana especificado"
type: docs
weight: 130
url: /es/net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

Establece períodos de tiempo predeterminados para el día de la semana especificado.

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| día | WeekDay | El día de la semana en el que establecer el día laborable predeterminado. |

## Ejemplos

Muestra cómo establecer un horario laboral predeterminado para un día.

```csharp
var project = new Project();

// Definir un calendar
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// Agregar días laborables de lunes a jueves con horarios predeterminados
var monday = new WeekDay(DayType.Monday);
WeekDay.SetDefaultWorkingTime(monday);
calendar.WeekDays.Add(monday);
var tuesday = new WeekDay(DayType.Tuesday);
WeekDay.SetDefaultWorkingTime(tuesday);
calendar.WeekDays.Add(tuesday);
var wednesday = new WeekDay(DayType.Wednesday);
WeekDay.SetDefaultWorkingTime(wednesday);
calendar.WeekDays.Add(wednesday);
var thursday = new WeekDay(DayType.Thursday);
WeekDay.SetDefaultWorkingTime(thursday);
calendar.WeekDays.Add(thursday);
var friday = new WeekDay(DayType.Friday);
WeekDay.SetDefaultWorkingTime(friday);
calendar.WeekDays.Add(friday);

var saturday = new WeekDay(DayType.Saturday);
saturday.DayWorking = false;
calendar.WeekDays.Add(saturday);
var sunday = new WeekDay(DayType.Sunday);
sunday.DayWorking = false;
calendar.WeekDays.Add(sunday);

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

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


