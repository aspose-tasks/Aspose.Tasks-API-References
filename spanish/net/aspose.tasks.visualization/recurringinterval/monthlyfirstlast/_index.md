---
title: "RecurringInterval.MonthlyFirstLast"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad RecurringInterval. Obtiene o establece un valor que indica si se deben mostrar líneas de progreso por el primer o último día predefinido"
type: docs
weight: 80
url: /es/net/aspose.tasks.visualization/recurringinterval/monthlyfirstlast/
---
## RecurringInterval.MonthlyFirstLast property

Obtiene o establece un valor que indica si se deben mostrar las líneas de progreso por el primer o último día predefinido.

```csharp
public bool MonthlyFirstLast { get; set; }
```

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

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


