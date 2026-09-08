---
title: "GanttChartView.MiddleTimescaleTier"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de GanttChartView. Obtiene o establece la configuración del nivel medio de escala de tiempo de la vista. TimescaleTier"
type: docs
weight: 100
url: /es/net/aspose.tasks/ganttchartview/middletimescaletier/
---
## GanttChartView.MiddleTimescaleTier property

Obtiene o establece la configuración del nivel medio de escala de tiempo de la vista. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier MiddleTimescaleTier { get; set; }
```

## Ejemplos

Muestra cómo trabajar con niveles de escala de tiempo mediante opciones de guardado.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

GanttChartView ganttChartView = (GanttChartView) project.Views.ToList()[0];

// establecer los niveles de escala de tiempo de la vista de diagrama de Gantt
ganttChartView.MiddleTimescaleTier.Unit = TimescaleUnit.Months;
ganttChartView.MiddleTimescaleTier.Count = 1;
ganttChartView.MiddleTimescaleTier.Label = DateLabel.MonthMmmm;

ganttChartView.BottomTimescaleTier.Unit = TimescaleUnit.Days;
ganttChartView.BottomTimescaleTier.Count = 1;
ganttChartView.BottomTimescaleTier.Label = DateLabel.DayDddDd;

// ...
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    Timescale = Timescale.DefinedInView
};

// ...

// guardar el proyecto como una imagen
project.Save(OutDir + "WorkWithTimescaleTier_out.png", options);
```

Muestra cómo modificar los niveles de escala de tiempo.

```csharp
var project = new Project();

// Inicializar vista Gantt Chart
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// establecer el recuento de escala de tiempo
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// agregar vista Gantt Chart al proyecto
project.Views.Add(view);

// agregar algunos datos de prueba al proyecto
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// Utilice la opción 'Timescale.DefinedInView' para renderizar escalas de tiempo usando la configuración de escala de tiempo que hemos establecido (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

Muestra cómo personalizar las etiquetas del nivel de escala de tiempo.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Agregar enlaces de tareas
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// ajustar los niveles de escala de tiempo

// ajustar el nivel superior
// establecer el nivel superior de escala de tiempo de la vista del diagrama de Gantt.
view.MiddleTimescaleTier = new TimescaleTier();
// establecer la unidad de escala de tiempo <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> para el nivel de escala de tiempo.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// establecer el intervalo de unidad de tiempo en el que se muestran las etiquetas para el nivel.
view.MiddleTimescaleTier.Count = 1;
// establecer la etiqueta de fecha <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> para el nivel de escala de tiempo.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// establecer cómo alinear las etiquetas dentro de cada período de tiempo del nivel (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// establecer un valor que indique si se deben mostrar marcas de verificación que separan los períodos de tiempo en el nivel.
view.MiddleTimescaleTier.ShowTicks = true;
// establecer un valor que indique si basar las etiquetas del nivel en el año fiscal.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// agregado para una mejor visualización
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// personalizar las fechas del nivel intermedio
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Utilizar la opción 'Timescale.DefinedInView' para representar escalas de tiempo usando la configuración de escalas de tiempo definida en la vista (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Ver también

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


