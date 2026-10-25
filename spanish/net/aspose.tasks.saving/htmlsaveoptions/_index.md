---
title: "Clase HtmlSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Saving.HtmlSaveOptions. Permite especificar opciones adicionales al renderizar páginas del proyecto a HTML"
type: docs
weight: 2010
url: /es/net/aspose.tasks.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Permite especificar opciones adicionales al renderizar páginas del proyecto a HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | Inicializa una nueva instancia de la clase `HtmlSaveOptions`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Obtiene o establece la lista de instancias de la clase [`BarStyle`](../../aspose.tasks.visualization/barstyle/) que aparecen en la vista del proyecto. |
| [CssSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | Obtiene o establece la función de devolución de llamada que se invoca para crear un recurso donde almacenar CSS. |
| [CssStylePrefix](../../aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/) { get; set; } | Obtiene o establece el prefijo de estilo CSS. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Obtiene o establece el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Obtiene o establece un valor que indica si el tiempo no laborable debe dibujarse (El valor predeterminado es TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Obtiene o establece una fecha para finalizar la renderización. |
| [ExportCss](../../aspose.tasks.saving/htmlsaveoptions/exportcss/) { get; set; } | Obtiene o establece la forma en que se exportan los CSS. |
| [ExportFonts](../../aspose.tasks.saving/htmlsaveoptions/exportfonts/) { get; set; } | Obtiene o establece la forma en que se exportan las fuentes. |
| [ExportImages](../../aspose.tasks.saving/htmlsaveoptions/exportimages/) { get; set; } | Obtiene o establece la forma en que se exportan las imágenes. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Obtiene o establece un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido. |
| [FontFaceTypes](../../aspose.tasks.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | Obtiene o establece los tipos de fuentes. |
| [FontSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | Obtiene o establece la función de devolución de llamada que se invoca para crear el recurso donde almacenar la fuente. |
| [FontSettings](../../aspose.tasks.saving/htmlsaveoptions/fontsettings/) { get; } | Especifica la configuración de fuentes utilizada al renderizar la vista del proyecto. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Obtiene o establece una lista de [`Gridline`](../../aspose.tasks.visualization/gridline/) que aparecen en la vista del proyecto. |
| [ImageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | Obtiene o establece la función de devolución de llamada que se invoca para crear el recurso donde almacenar la fuente. |
| [IncludeProjectNameInPageHeader](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameinpageheader/) { get; set; } | Obtiene o establece un valor que indica si se debe incluir el nombre del proyecto en el encabezado de la página HTML. |
| [IncludeProjectNameInTitle](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/) { get; set; } | Obtiene o establece un valor que indica si se debe incluir el nombre del proyecto en el título HTML. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Obtiene o establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Obtiene o establece un valor que define cómo renderizar una leyenda. El valor predeterminado es LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Obtiene o establece una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de la página. Si es null, se renderizan los elementos predeterminados. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Obtiene o establece un valor que indica si las tareas críticas deben mostrarse en color rojo (El valor predeterminado es FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Obtiene o establece el color del tiempo no laborable. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Obtiene o establece el número de páginas del proyecto. |
| [Pages](../../aspose.tasks.saving/htmlsaveoptions/pages/) { get; set; } | Obtiene o establece una lista de números de página para guardar al renderizar el diseño del proyecto. Todas las páginas del proyecto se guardarán si esta lista está vacía. |
| [PageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | Obtiene o establece una función de devolución de llamada definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Obtiene o establece el tamaño de la página a renderizar (El valor predeterminado es PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Obtiene o establece el [`PresentationFormat`](../saveoptions/presentationformat/) en el que se guardará el documento. |
| [ReduceFooterGap](../../aspose.tasks.saving/htmlsaveoptions/reducefootergap/) { get; set; } | Obtiene o establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página. |
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
| override [UseGradientBrush](../../aspose.tasks.saving/htmlsaveoptions/usegradientbrush/) { get; set; } | Obtiene o establece un valor que indica si se debe usar un pincel degradado al renderizar el diseño del proyecto. Actualmente, el uso de pincel degradado no es compatible al renderizar a HTML. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Obtiene o establece una lista de las columnas de vista a renderizar ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Si no se establece, solo se renderizan los IDs de tarea, los nombres de tarea, el inicio y el fin. Si se establecen tanto la propiedad View como las propiedades de [`ViewSettings`](../saveoptions/viewsettings/), las columnas de View sobrescriben a las columnas de ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Obtiene o establece una vista ([`View`](../saveoptions/view/)) para renderizar. Puede usar esta opción para especificar explícitamente qué vista debe guardarse en formatos PDF, HTML o Imagen. Si se establece esta propiedad, la propiedad [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) se ignora al guardar el proyecto. La vista debe provenir de una de las siguientes pantallas (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## Ejemplos

Muestra cómo guardar un proyecto en formato HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// O

// Añadiendo solo una página (número de página 2)
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### Ver también

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


