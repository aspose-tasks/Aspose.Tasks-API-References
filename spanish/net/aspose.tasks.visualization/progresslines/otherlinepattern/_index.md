---
title: "ProgressLines.OtherLinePattern"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ProgressLines. Obtiene o establece el patrón de línea para otra línea de progreso"
type: docs
weight: 130
url: /es/net/aspose.tasks.visualization/progresslines/otherlinepattern/
---
## ProgressLines.OtherLinePattern property

Obtiene o establece el patrón de línea para otra línea de progreso.

```csharp
public LinePattern OtherLinePattern { get; set; }
```

## Ejemplos

Muestra cómo trabajar con líneas de progreso.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// definamos la línea de progreso
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// establezca la fecha a partir de la cual mostrar las líneas de progreso. Definamos la fecha de estado de un proyecto.
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// establezca un valor que indique si se deben mostrar las líneas de progreso desde el inicio de la fecha de comienzo del proyecto
progressLines.BeginAtProjectStart = true;
// establezca el formato de fecha (<see cref="T:Aspose.Tasks.Visualization.DateLabel" />).
progressLines.DateFormat = DateLabel.DayDddd;
// establezca un valor que indique si se debe mostrar la línea de progreso en la fecha actual.
progressLines.DisplayAtCurrentDate = true;
// establezca un valor que indique si se debe mostrar la línea de progreso en intervalos recurrentes.
progressLines.DisplayAtRecurringIntervals = true;
// establezca un valor que indique si se deben mostrar las líneas de progreso en las fechas seleccionadas
progressLines.DisplaySelected = true;
// establezca un valor que indique si se deben mostrar las líneas de progreso para el plan base o real.
progressLines.IsBaselinePlan = false;
// establezca la fuente utilizada para la etiqueta de la línea de progreso.
progressLines.Font = new FontDescriptor("Arial", 10);
// establezca el color de línea para la línea de progreso actual.
progressLines.LineColor = Color.Aquamarine;
// establezca el patrón de línea de la línea de progreso actual.
progressLines.LinePattern = LinePattern.Dashed;
// establezca el color de otra línea de progreso.
progressLines.OtherLineColor = Color.Azure;
// establezca el patrón de línea para otra línea de progreso.
progressLines.OtherLinePattern = LinePattern.Dotted;
// establezca el color de otro punto de progreso.
progressLines.OtherProgressPointColor = Color.Red;
// establezca la forma del punto de progreso de otra línea de progreso.
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// establezca el color del punto de progreso.
progressLines.ProgressPointColor = Color.Orange;
// establecer la forma del punto de progreso.
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// establecer el intervalo recurrente.
progressLines.RecurringInterval = new RecurringInterval();
// establecer el intervalo recurrente.
progressLines.RecurringInterval.Interval = Interval.Daily;
// establecer el número de día diario
progressLines.RecurringInterval.DailyDayNumber = 1;
// establecer un valor que indica si se muestra la fecha para cada línea de progreso.
progressLines.ShowDate = true;

// veamos las líneas de progreso
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* enum [LinePattern](../../linepattern/)
* class [ProgressLines](../)
* namespace [Aspose.Tasks.Visualization](../../progresslines/)
* assembly [Aspose.Tasks](../../../)


