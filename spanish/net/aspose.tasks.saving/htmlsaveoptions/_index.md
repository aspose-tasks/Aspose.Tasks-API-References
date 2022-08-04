---
title: HtmlSaveOptions
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Permite especificar opciones adicionales al renderizar páginas de proyecto a HTML.
type: docs
weight: 1740
url: /es/net/aspose.tasks.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Permite especificar opciones adicionales al renderizar páginas de proyecto a HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions)() | Inicializa una nueva instancia del[`HtmlSaveOptions`](../htmlsaveoptions) clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Obtiene o establece la lista de las instancias del[`BarStyle`](../../aspose.tasks.visualization/barstyle) class que aparecen en la vista del proyecto. |
| [CssSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/csssavingcallback) { get; set; } | Obtiene o establece la devolución de llamada que se llama para crear un recurso para almacenar CSS. |
| [CssStylePrefix](../../aspose.tasks.saving/htmlsaveoptions/cssstyleprefix) { get; set; } | Obtiene o establece el prefijo de estilo CSS. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Obtiene o establece el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada). |
| [DefaultFontName](../../aspose.tasks.saving/htmlsaveoptions/defaultfontname) { get; set; } | Obtiene o establece la fuente predeterminada para renderizar. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Obtiene o establece un valor que indica si se debe dibujar el tiempo no laborable (el valor predeterminado es VERDADERO). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Obtiene o establece una fecha para terminar de renderizar. |
| [ExportCss](../../aspose.tasks.saving/htmlsaveoptions/exportcss) { get; set; } | Obtiene o establece la forma en que se exportan los CSS. |
| [ExportFonts](../../aspose.tasks.saving/htmlsaveoptions/exportfonts) { get; set; } | Obtiene o establece la forma en que se exportan las fuentes. |
| [ExportImages](../../aspose.tasks.saving/htmlsaveoptions/exportimages) { get; set; } | Obtiene o establece la forma en que se exportan las imágenes. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Obtiene o establece un valor que indica si se debe aumentar el alto de la fila para que se ajuste a su contenido. |
| [FontFaceTypes](../../aspose.tasks.saving/htmlsaveoptions/fontfacetypes) { get; set; } | Obtiene o establece los tipos de letra de la fuente. |
| [FontResolveCallback](../../aspose.tasks.saving/htmlsaveoptions/fontresolvecallback) { get; set; } | Obtiene o establece una devolución de llamada que se puede usar para personalizar las fuentes resueltas. |
| [FontSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/fontsavingcallback) { get; set; } | Obtiene o establece la devolución de llamada que se llama para crear un recurso para almacenar la fuente. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Obtiene o establece una lista de[`Gridline`](../../aspose.tasks.visualization/gridline) que aparecen en la vista del proyecto. |
| [ImageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/imagesavingcallback) { get; set; } | Obtiene o establece la devolución de llamada que se llama para crear un recurso para almacenar la fuente. |
| [IncludeProjectNameInPageHeader](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameinpageheader) { get; set; } | Obtiene o establece un valor que indica si se debe incluir el nombre del proyecto en el encabezado de la página HTML. |
| [IncludeProjectNameInTitle](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle) { get; set; } | Obtiene o establece un valor que indica si se debe incluir el nombre del proyecto en el título HTML. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Obtiene o establece un valor que indica si la leyenda debe mostrarse en cada página (el valor predeterminado es VERDADERO). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Obtiene o establece un valor que indica si las tareas críticas deben mostrarse en color rojo (el valor predeterminado es FALSO). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Obtiene o establece el color del tiempo no laborable. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Obtiene o establece el número de páginas del proyecto. |
| [Pages](../../aspose.tasks.saving/htmlsaveoptions/pages) { get; set; } | Obtiene o establece una lista de números de página para guardar al renderizar el diseño del proyecto. Todas las páginas del proyecto se guardarán si esta lista está vacía. |
| [PageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/pagesavingcallback) { get; set; } | Obtiene o establece una devolución de llamada definida por el usuario que se usa para obtener un flujo de salida para cada página renderizada. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | Obtiene o establece el tamaño de la página que se representará (el valor predeterminado es PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Obtiene o establece el[`PresentationFormat`](../saveoptions/presentationformat) en el que se guardará el documento. |
| [ReduceFooterGap](../../aspose.tasks.saving/htmlsaveoptions/reducefootergap) { get; set; } | Obtiene o establece un valor que indica si se debe reducir un espacio entre la última tarea y el pie de página. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Obtiene o establece un valor que indica si un proyecto debe representarse en una sola página cuando el proyecto se guarda en formato gráfico. El tamaño de la página cambiará para que el proyecto representado pueda caber en una sola página. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Obtiene o establece un valor que indica si se deben marcar las subtareas en la barra de tareas de resumen. Para las subtareas, el campo Resumen indica si la información de las barras de Gantt de las subtareas se acumulará en la barra de tareas de resumen. Para las tareas de resumen, el campo Resumen El campo indica si la barra de tareas de resumen muestra barras acumuladas. Debe tener el campo Resumen para tareas de resumen establecido en Sí para que cualquier subtarea se acumule en ellas. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Obtiene o establece el formato en el que se guardará el documento si se utiliza este objeto de opciones de guardado. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Obtiene o establece la fecha desde la que se empieza a renderizar. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Obtiene o establece el comparador para ordenar tareas en diagramas de Gantt y hojas de tareas. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Obtiene o establece la condición que se usa para filtrar tareas representadas en diagramas de Gantt, hoja de tareas y uso de tareas. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Obtiene o establece la lista de las instancias del[`TextStyle`](../../aspose.tasks.visualization/textstyle) class que aparecen en la vista del proyecto. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Obtiene o establece el[`Timescale`](../saveoptions/timescale) valor que se usa para controlar cómo se representa la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico. |
| override [UseGradientBrush](../../aspose.tasks.saving/htmlsaveoptions/usegradientbrush) { get; set; } | Obtiene o establece un valor que indica si se debe usar el pincel de degradado al renderizar el diseño del proyecto. Actualmente, no se admite el uso de un pincel degradado cuando se renderiza a HTML. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/htmlsaveoptions/useprojectdefaultfont) { get; set; } | Obtiene o establece un valor que indica si se debe utilizar la fuente predeterminada para la representación. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | Obtiene o establece una lista de las columnas de vista para representar ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn) ). Si no se establece, solo se representan los ID de tarea, los nombres de tarea, el inicio y el final. Si tanto Ver como[`ViewSettings`](../saveoptions/viewsettings) las propiedades están configuradas, las columnas de View reemplazan las columnas de ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Obtiene o establece una vista ([`View`](../saveoptions/view) para renderizar. Puede usar estas opciones para especificar explícitamente qué vista debe guardarse en formato PDF, HTML o de imagen. Si se establece esta propiedad,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) La propiedad se ignora cuando se guarda el proyecto. La vista debe ser desde una de las siguientes pantallas (([`Screen`](../../aspose.tasks/view/screen) )): (Gantt, Hoja de tareas, Uso de tareas, Hoja de recursos, Uso de recursos) |

### Ver también

* class [SaveOptions](../saveoptions)
* espacio de nombres [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* asamblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
