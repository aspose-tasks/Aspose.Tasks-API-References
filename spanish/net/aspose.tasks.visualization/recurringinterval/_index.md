---
title: "Clase RecurringInterval"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.RecurringInterval. Representa intervalos recurrentes usados en líneas de progreso de una vista de diagrama de Gantt"
type: docs
weight: 3310
url: /es/net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

Representa intervalos recurrentes usados en líneas de progreso de una vista de diagrama de Gantt.

```csharp
public class RecurringInterval
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | Obtiene o establece el número del día diario. |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | Obtiene o establece un valor que indica si un día es laborable para las líneas de progreso diarias. |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | Obtiene o establece el intervalo recurrente. Puede ser cualquier valor del tipo [`Interval`](./interval/). |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | Obtiene o establece un valor que indica si mostrar líneas de progreso mensuales por día. |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | Obtiene o establece el número de día de las líneas de progreso mensuales. |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | Obtiene o establece el número de mes de las líneas de progreso mensuales. |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar las líneas de progreso por el primer o último día predefinido. |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | Obtiene o establece el tipo de día primero o último de las líneas de progreso mensuales. |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | Obtiene o establece el número de mes de las líneas de progreso, que se muestran por el primer o último día predefinido. |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | Obtiene una lista de días para las líneas de progreso semanales. |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | Obtiene o establece el número de semana para las líneas de progreso semanales. |

## Ejemplos

Muestra cómo trabajar con intervalos recurrentes de líneas de progreso.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// permite leer la línea de progreso
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// permite redefinir el intervalo recurrente
var newInterval = new RecurringInterval();

// establece un valor que indica si se deben mostrar líneas de progreso mensuales por día.
interval.MonthlyDay = true;
// establece el número de día de las líneas de progreso mensuales.
interval.MonthlyDayDayNumber = 1;
// establece el número de mes de las líneas de progreso mensuales.
interval.MonthlyDayMonthNumber = 1;
// establece un valor que indica si se deben mostrar líneas de progreso por el primer o último día predefinido.
interval.MonthlyFirstLast = true;
// establece el tipo de primer o último día de las líneas de progreso mensuales.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// establece el número de mes de las líneas de progreso, que se muestran por el primer o último día predefinido.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


