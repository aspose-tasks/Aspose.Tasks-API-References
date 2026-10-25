---
title: "Clase SvgOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Saving.SvgOptions. Permite especificar opciones adicionales al renderizar las páginas del proyecto a SVG."
type: docs
weight: 2230
url: /es/net/aspose.tasks.saving/svgoptions/
---
## SvgOptions class

Permite especificar opciones adicionales al renderizar páginas de proyecto a SVG.

```csharp
public class SvgOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SvgOptions](svgoptions/)() | Inicializa una nueva instancia de la clase `SvgOptions` que puede usarse para guardar el proyecto en formato SVG. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Obtiene o establece la lista de instancias de la clase [`BarStyle`](../../aspose.tasks.visualization/barstyle/) que aparecen en la vista del proyecto. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Obtiene o establece el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Obtiene o establece un valor que indica si el tiempo no laborable debe dibujarse (El valor predeterminado es TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Obtiene o establece una fecha para finalizar la renderización. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Obtiene o establece un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Obtiene o establece una lista de [`Gridline`](../../aspose.tasks.visualization/gridline/) que aparecen en la vista del proyecto. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Obtiene o establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Obtiene o establece un valor que define cómo renderizar una leyenda. El valor predeterminado es LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Obtiene o establece una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de la página. Si es null, se renderizan los elementos predeterminados. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Obtiene o establece un valor que indica si las tareas críticas deben mostrarse en color rojo (El valor predeterminado es FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Obtiene o establece el color del tiempo no laborable. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Obtiene o establece el número de páginas del proyecto. |
| [PageSavingCallback](../../aspose.tasks.saving/svgoptions/pagesavingcallback/) { get; set; } | Obtiene o establece una devolución de llamada de implementación definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Obtiene o establece el tamaño de la página a renderizar (El valor predeterminado es PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Obtiene o establece el [`PresentationFormat`](../saveoptions/presentationformat/) en el que se guardará el documento. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Obtiene o establece un valor que indica si un proyecto debe renderizarse en una sola página cuando el proyecto se guarda en formato gráfico. El tamaño de la página se cambiará para que el proyecto renderizado quepa en una sola página. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Obtiene o establece un valor que indica si las subtareas en la barra de tarea resumida deben marcarse. Para las subtareas, el campo Rollup indica si la información de las barras Gantt de la subtarea se consolidará en la barra de tarea resumida. Para las tareas resumidas, el campo Rollup indica si la barra de tarea resumida muestra barras consolidadas. Debe tener el campo Rollup de las tareas resumidas configurado en Yes para que cualquier subtarea se consolide en ellas. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtiene o establece el formato en el que se guardará el documento si se utiliza este objeto de opciones de guardado. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Obtiene o establece la fecha a partir de la cual iniciar la renderización. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Obtiene o establece una devolución de llamada que puede usarse para personalizar algunos aspectos de la renderización de enlaces de tareas. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtiene o establece el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtiene o establece la condición que se utiliza para filtrar las tareas renderizadas en los diagramas de Gantt, hoja de tareas y uso de tareas. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Obtiene o establece la lista de estilos de texto que se aplican durante la renderización de una vista de proyecto. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Obtiene o establece el valor de [`Timescale`](../saveoptions/timescale/) que se usa para controlar cómo se renderiza la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Obtiene o establece un comportamiento que define cómo alinear el extremo derecho de la escala de tiempo con el final de la página. |
| override [UseGradientBrush](../../aspose.tasks.saving/svgoptions/usegradientbrush/) { get; set; } | Determina si se debe usar un pincel degradado al renderizar el diseño del proyecto. Actualmente, el uso de pincel degradado no es compatible con el renderizado a SVG. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Obtiene o establece una lista de las columnas de vista a renderizar ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Si no se establece, solo se renderizan los IDs de tarea, los nombres de tarea, el inicio y el fin. Si se establecen tanto la propiedad View como las propiedades de [`ViewSettings`](../saveoptions/viewsettings/), las columnas de View sobrescriben a las columnas de ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Obtiene o establece una vista ([`View`](../saveoptions/view/)) para renderizar. Puede usar esta opción para especificar explícitamente qué vista debe guardarse en formatos PDF, HTML o Imagen. Si se establece esta propiedad, la propiedad [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) se ignora al guardar el proyecto. La vista debe provenir de una de las siguientes pantallas (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## Ejemplos

Muestra cómo guardar el proyecto como archivo SVG.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // establece el <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> en el que se guardará el documento
                            PresentationFormat = PresentationFormat.GanttChart,

                            // establece un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido
                            FitContent = true,

                            // establece el período de tiempo mínimo para renderizar. El valor predeterminado es <see cref="P:Aspose.Tasks.Saving.SaveOptions.Timescale">Days</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // determina si se debe usar un pincel degradado al renderizar el diseño del proyecto
                            // Actualmente, el uso de pincel degradado no es compatible con el renderizado a SVG.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### Ver también

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


