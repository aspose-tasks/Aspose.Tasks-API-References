---
title: "Clase TimelineView"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TimelineView. Representa una vista de línea de tiempo de un proyecto"
type: docs
weight: 2580
url: /es/net/aspose.tasks/timelineview/
---
## TimelineView class

Representa una vista de línea de tiempo de un proyecto.

```csharp
public class TimelineView : View
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TimelineView](timelineview/)() | Inicializa una nueva instancia de la clase `TimelineView`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DateFormat](../../aspose.tasks/timelineview/dateformat/) { get; set; } | Obtiene o establece un valor que indica cómo formatear las fechas en la vista Timeline. |
| [DisplayOverlapped](../../aspose.tasks/timelineview/displayoverlapped/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar tareas superpuestas en varias filas. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Obtiene o establece un filtro utilizado en una vista única. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Obtiene o establece un grupo de la vista única. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Obtiene o establece un valor que indica si Microsoft Project resalta el filtro para una vista única. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Obtiene o establece el nombre de un objeto View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Obtiene una instancia de la clase [`PageInfo`](../view/pageinfo/). Representa los datos de configuración de página que están presentes en el formato de archivo mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Obtiene el padre del objeto View. Solo lectura [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Obtiene el tipo de pantalla para la vista única. Solo lectura [`ViewScreen`](../viewscreen/). |
| [ShowDates](../../aspose.tasks/timelineview/showdates/) { get; } | Obtiene un valor que indica si se deben mostrar fechas. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Obtiene o establece un valor que indica si Microsoft Project muestra el nombre de la vista única en las listas desplegables Vista u Otras Vistas en la cinta de opciones. |
| [ShowPanZoom](../../aspose.tasks/timelineview/showpanzoom/) { get; set; } | Obtiene o establece un valor que indica si se debe mostrar el control de panorámica y zoom. |
| [ShowTimescale](../../aspose.tasks/timelineview/showtimescale/) { get; set; } | Obtiene o establece un valor que indica si se debe mostrar la escala de tiempo. |
| [ShowToday](../../aspose.tasks/timelineview/showtoday/) { get; set; } | Obtiene o establece un valor que indica si se debe mostrar una línea que representa el día de hoy. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Obtiene o establece una tabla de la vista única. |
| [TextLinesCount](../../aspose.tasks/timelineview/textlinescount/) { get; set; } | Obtiene o establece un valor que indica cuántas líneas se usan para mostrar la tarea en una línea de tiempo. |
| [Type](../../aspose.tasks/view/type/) { get; } | Obtiene el tipo de elemento en la vista única, como tareas o recursos. Solo lectura [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Obtiene el identificador único de una vista. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Obtiene una colección de objetos que representan la ubicación y apariencia de [`OleObject`](../oleobject/) en la vista. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Compara la instancia actual con otro objeto del mismo tipo y devuelve un entero que indica si la instancia actual precede, sigue o se encuentra en la misma posición en el orden de clasificación que el otro objeto. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Devuelve un valor de código hash para la instancia de la clase [`Resource`](../resource/). |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


