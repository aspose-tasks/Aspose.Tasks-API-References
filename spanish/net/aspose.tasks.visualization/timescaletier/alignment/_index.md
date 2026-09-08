---
title: "TimescaleTier.Alignment"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TimescaleTier. Obtiene o establece cómo alinear las etiquetas dentro de cada período de tiempo del nivel HorizontalStringAlignment"
type: docs
weight: 20
url: /es/net/aspose.tasks.visualization/timescaletier/alignment/
---
## TimescaleTier.Alignment property

Obtiene o establece cómo alinear las etiquetas dentro de cada período de tiempo del nivel ([`HorizontalStringAlignment`](../../horizontalstringalignment/)).

```csharp
public HorizontalStringAlignment Alignment { get; set; }
```

## Ejemplos

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

* enum [HorizontalStringAlignment](../../horizontalstringalignment/)
* class [TimescaleTier](../)
* namespace [Aspose.Tasks.Visualization](../../timescaletier/)
* assembly [Aspose.Tasks](../../../)


