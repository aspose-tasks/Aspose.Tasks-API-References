---
title: "Enum TimeUnitType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.TimeUnitType enum. Especifica el tipo de una unidad de tiempo"
type: docs
weight: 2570
url: /es/net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

Especifica el tipo de una unidad de tiempo.

```csharp
public enum TimeUnitType : sbyte
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | Indica que el valor Undefined significa que el campo no fue definido en el archivo de proyecto original. |
| Minute | `0` | Indica el tipo de unidad de tiempo Minuto. |
| ElapsedMinute | `1` | Indica el tipo de unidad de tiempo minuto transcurrido. |
| Hour | `2` | Indica el tipo de unidad de tiempo Hora. |
| ElapsedHour | `3` | Indica el tipo de unidad de tiempo hora transcurrida. |
| Day | `4` | Indica el tipo de unidad de tiempo Día. |
| ElapsedDay | `5` | Indica el tipo de unidad de tiempo día transcurrido. |
| Week | `6` | Indica el tipo de unidad de tiempo Semana. |
| ElapsedWeek | `7` | Indica el tipo de unidad de tiempo semana transcurrida. |
| Month | `8` | Indica el tipo de unidad de tiempo Mes. |
| ElapsedMonth | `9` | Indica el tipo de unidad de tiempo mes transcurrido. |
| Percent | `10` | Indica el tipo de unidad de tiempo Porcentaje. |
| ElapsedPercent | `11` | Indica el tipo de unidad de tiempo porcentaje transcurrido. |
| Null | `12` | Indica el tipo de unidad de tiempo Null. |
| MinuteEstimated | `13` | Indica el tipo de unidad de tiempo estimado Minuto. |
| ElapsedMinuteEstimated | `14` | Indica el tipo de unidad de tiempo estimado minuto transcurrido. |
| HourEstimated | `15` | Indica el tipo de unidad de tiempo estimado Hora. |
| ElapsedHourEstimated | `16` | Indica el tipo de unidad de tiempo estimado hora transcurrida. |
| DayEstimated | `17` | Indica el tipo de unidad de tiempo estimado Día. |
| ElapsedDayEstimated | `18` | Indica el tipo de unidad de tiempo estimado día transcurrido. |
| WeekEstimated | `19` | Indica el tipo de unidad de tiempo estimado Semana. |
| ElapsedWeekEstimated | `20` | Indica el tipo de unidad de tiempo estimado semana transcurrida. |
| MonthEstimated | `21` | Indica el tipo de unidad de tiempo estimado Mes. |
| ElapsedMonthEstimated | `22` | Indica el tipo de unidad de tiempo estimado mes transcurrido. |
| PercentEstimated | `23` | Indica el tipo de unidad de tiempo estimado Porcentaje. |
| ElapsedPercentEstimated | `24` | Indica el tipo de unidad de tiempo estimado en porcentaje transcurrido. |
| Year | `25` | Indica el tipo de unidad de tiempo Año. |

## Observaciones

Al exportar a XML, los valores Undefined se eliminarán del XML resultante.

## Ejemplos

Muestra cómo convertir una duración en diferentes tipos de unidades de tiempo.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Obtén una tarea para calcular su duración en diferentes formatos
var task = project.RootTask.Children.GetById(1);

// Obtén la duración en Minutos, Días, Horas, Semanas y Meses
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


