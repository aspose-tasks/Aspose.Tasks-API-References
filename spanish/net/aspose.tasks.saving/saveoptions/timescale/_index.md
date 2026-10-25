---
title: "SaveOptions.Timescale"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece el valor Timescale que se utiliza para controlar cómo se renderiza la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico."
type: docs
weight: 200
url: /es/net/aspose.tasks.saving/saveoptions/timescale/
---
## SaveOptions.Timescale property

Obtiene o establece el valor `Timescale` que se utiliza para controlar cómo se renderiza la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico.

```csharp
public Timescale Timescale { get; set; }
```

## Ejemplos

Muestra cómo establecer el período de tiempo mínimo a renderizar. El valor predeterminado es &lt;see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\"&gt;Days&lt;/see&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Guardar en una imagen de una página (Timescale.days por defecto)
project.Save(OutDir + "NewProductDevDays_out.jpeg", new ImageSaveOptions(SaveFileFormat.Jpeg));

// Guardar en una imagen de una página (Timescale.ThirdsOfMonths)
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "NewProductDevThirdsOfMonths_out.jpeg", options);

// Guardar en una imagen de una página (Timescale.Months)
options.Timescale = Timescale.Months;
project.Save(OutDir + "NewProductDevMonths_out.jpeg", options);
```

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

Muestra cómo renderizar la vista de uso de tareas con la configuración de escala de tiempo definida en la configuración de la vista.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// Defina las SaveOptions y especifique que se deben usar los ajustes de escala de tiempo de TaskUsageView.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
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

### Ver también

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


