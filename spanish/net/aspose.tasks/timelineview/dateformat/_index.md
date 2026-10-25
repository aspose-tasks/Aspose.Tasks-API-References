---
title: "TimelineView.DateFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TimelineView. Obtiene o establece un valor que indica cómo formatear las fechas en la vista de línea de tiempo"
type: docs
weight: 20
url: /es/net/aspose.tasks/timelineview/dateformat/
---
## TimelineView.DateFormat property

Obtiene o establece un valor que indica cómo formatear las fechas en la vista Timeline.

```csharp
public DateFormat DateFormat { get; set; }
```

## Ejemplos

Muestra cómo trabajar con &lt;see cref="Aspose.Tasks.TimelineView" /&gt;.

```csharp
var project = new Project();

// inicializar una vista de línea de tiempo
var view = new TimelineView();

// establecer un valor que indica cómo formatear las fechas en la vista Timeline.
view.DateFormat = DateFormat.DateDddDd;
// establecer un valor que indica si se deben mostrar tareas superpuestas en varias filas.
view.DisplayOverlapped = true;
// establecer un valor que indica si se debe mostrar el control de panorámica y zoom.
view.ShowPanZoom = true;
// establecer un valor que indica si se debe mostrar la escala de tiempo.
view.ShowTimescale = true;
// establecer un valor que indica si se debe mostrar una línea que representa el día de hoy.
view.ShowToday = true;
// establecer un valor que indica cuántas líneas se usan para mostrar la tarea en una línea de tiempo.
view.TextLinesCount = 2;

// obtiene un valor que indica si se deben mostrar tareas superpuestas en varias filas.
Console.WriteLine("Show Dates: " + view.ShowDates);

// agregar la vista al proyecto
project.Views.Add(view);

// agregar algunos datos de prueba al proyecto
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### Ver también

* enum [DateFormat](../../dateformat/)
* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)


