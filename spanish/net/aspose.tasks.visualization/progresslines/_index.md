---
title: "Clase ProgressLines"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.ProgressLines. Representa líneas de progreso en una vista de diagrama de Gantt"
type: docs
weight: 3290
url: /es/net/aspose.tasks.visualization/progresslines/
---
## ProgressLines class

Representa líneas de progreso en una vista de diagrama de Gantt.

```csharp
public class ProgressLines
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ProgressLines](progresslines/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BeginAtDate](../../aspose.tasks.visualization/progresslines/beginatdate/) { get; set; } | Obtiene o establece la fecha desde la cual mostrar las líneas de progreso. |
| [BeginAtProjectStart](../../aspose.tasks.visualization/progresslines/beginatprojectstart/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar las líneas de progreso desde el inicio de la fecha de comienzo del proyecto. |
| [DateFormat](../../aspose.tasks.visualization/progresslines/dateformat/) { get; set; } | Obtiene o establece el formato de fecha ([`DateLabel`](../datelabel/)). |
| [DisplayAtCurrentDate](../../aspose.tasks.visualization/progresslines/displayatcurrentdate/) { get; set; } | Obtiene o establece un valor que indica si se debe mostrar la línea de progreso en la fecha actual. |
| [DisplayAtRecurringIntervals](../../aspose.tasks.visualization/progresslines/displayatrecurringintervals/) { get; set; } | Obtiene o establece un valor que indica si se debe mostrar la línea de progreso en intervalos recurrentes. |
| [DisplaySelected](../../aspose.tasks.visualization/progresslines/displayselected/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar las líneas de progreso en las fechas seleccionadas. |
| [Font](../../aspose.tasks.visualization/progresslines/font/) { get; set; } | Obtiene o establece la fuente utilizada para la etiqueta de la línea de progreso. |
| [IsBaselinePlan](../../aspose.tasks.visualization/progresslines/isbaselineplan/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar las líneas de progreso para el plan base o real. |
| [LineColor](../../aspose.tasks.visualization/progresslines/linecolor/) { get; set; } | Obtiene o establece el color de línea para la línea de progreso actual. |
| [LinePattern](../../aspose.tasks.visualization/progresslines/linepattern/) { get; set; } | Obtiene o establece el patrón de línea de la línea de progreso actual. [`LinePattern`](./linepattern/). |
| [OtherLineColor](../../aspose.tasks.visualization/progresslines/otherlinecolor/) { get; set; } | Obtiene o establece el color de otra línea de progreso. |
| [OtherLinePattern](../../aspose.tasks.visualization/progresslines/otherlinepattern/) { get; set; } | Obtiene o establece el patrón de línea para otra línea de progreso. |
| [OtherProgressPointColor](../../aspose.tasks.visualization/progresslines/otherprogresspointcolor/) { get; set; } | Obtiene o establece el color de otro punto de progreso. |
| [OtherProgressPointShape](../../aspose.tasks.visualization/progresslines/otherprogresspointshape/) { get; set; } | Obtiene o establece la forma del punto de progreso de otra línea de progreso. |
| [ProgressPointColor](../../aspose.tasks.visualization/progresslines/progresspointcolor/) { get; set; } | Obtiene o establece el color del punto de progreso. |
| [ProgressPointShape](../../aspose.tasks.visualization/progresslines/progresspointshape/) { get; set; } | Obtiene o establece la forma del punto de progreso. [`GanttBarEndShape`](../ganttbarendshape/). |
| [RecurringInterval](../../aspose.tasks.visualization/progresslines/recurringinterval/) { get; set; } | Obtiene o establece el intervalo recurrente. [`RecurringInterval`](./recurringinterval/). |
| [SelectedDates](../../aspose.tasks.visualization/progresslines/selecteddates/) { get; } | Obtiene la lista de fechas seleccionadas para mostrar líneas de progreso. |
| [ShowDate](../../aspose.tasks.visualization/progresslines/showdate/) { get; set; } | Obtiene o establece un valor que indica si se muestra la fecha para cada línea de progreso. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


