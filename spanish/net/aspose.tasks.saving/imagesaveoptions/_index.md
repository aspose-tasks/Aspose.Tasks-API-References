---
title: Class ImageSaveOptions
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Aspose.Tasks.Saving.ImageSaveOptions clase. Permite especificar opciones adicionales al representar páginas de proyecto en imágenes.
type: docs
weight: 1770
url: /es/net/aspose.tasks.saving/imagesaveoptions/
---
## ImageSaveOptions class

Permite especificar opciones adicionales al representar páginas de proyecto en imágenes.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFileFormat) | Inicializa una nueva instancia del`ImageSaveOptions` clase que se puede utilizar para guardar imágenes renderizadas en formatos TIFF, PNG, BMP o JPEG. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Obtiene o establece la lista de las instancias del[`BarStyle`](../../aspose.tasks.visualization/barstyle/) class que aparecen en la vista del proyecto. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Obtiene o establece el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada). |
| [DefaultFontName](../../aspose.tasks.saving/imagesaveoptions/defaultfontname/) { get; set; } | Obtiene o establece la fuente predeterminada para renderizar. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Obtiene o establece un valor que indica si se debe dibujar el tiempo no laborable (el valor predeterminado es VERDADERO). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Obtiene o establece una fecha para terminar de renderizar. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Obtiene o establece un valor que indica si se debe aumentar el alto de la fila para que se ajuste a su contenido. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | Obtiene o establece si una sección de calendario de una vista debe representarse al final (lado derecho) de la última página. Si el valor es falso, la sección de calendario se representa exactamente en EndDate, incluso si hay un espacio vacío en una página. |
| [FontResolveCallback](../../aspose.tasks.saving/imagesaveoptions/fontresolvecallback/) { get; set; } | Obtiene o establece una devolución de llamada que se puede usar para personalizar las fuentes resueltas. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Obtiene o establece una lista de[`Gridline`](../../aspose.tasks.visualization/gridline/) que aparecen en la vista del proyecto. |
| [HorizontalResolution](../../aspose.tasks.saving/imagesaveoptions/horizontalresolution/) { get; set; } | Obtiene o establece la resolución horizontal en dpi. |
| [JpegQuality](../../aspose.tasks.saving/imagesaveoptions/jpegquality/) { get; set; } | Obtiene o establece una calidad JPEG. El rango de valores permitido es 0..100. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | Obtiene o establece un valor que indica si la leyenda debe mostrarse en cada página (el valor predeterminado es VERDADERO). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Obtiene o establece un valor que indica si las tareas críticas deben mostrarse en color rojo (el valor predeterminado es FALSO). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Obtiene o establece el color del tiempo no laborable. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Obtiene o establece el número de páginas del proyecto. |
| [Pages](../../aspose.tasks.saving/imagesaveoptions/pages/) { get; set; } | Obtiene o establece una lista de números de página para guardar al guardar el diseño del proyecto en archivos separados. Todas las páginas se guardarán si esta lista está vacía. |
| [PageSavingCallback](../../aspose.tasks.saving/imagesaveoptions/pagesavingcallback/) { get; set; } | Obtiene o establece una devolución de llamada definida por el usuario que se usa para obtener un flujo de salida para cada página renderizada. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Obtiene o establece el tamaño de la página que se representará (el valor predeterminado es PageSize.A4). |
| [PixelFormat](../../aspose.tasks.saving/imagesaveoptions/pixelformat/) { get; set; } | Obtiene o establece el formato de los datos de color para cada píxel de la imagen. |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Obtiene o establece el[`PresentationFormat`](../saveoptions/presentationformat/) en el que se guardará el documento. |
| [ReduceFooterGap](../../aspose.tasks.saving/imagesaveoptions/reducefootergap/) { get; set; } | Obtiene o establece un valor que indica si se debe reducir un espacio entre la última tarea y el pie de página. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Obtiene o establece un valor que indica si un proyecto debe representarse en una sola página cuando el proyecto se guarda en formato gráfico. El tamaño de la página cambiará para que el proyecto representado pueda caber en una sola página. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Obtiene o establece un valor que indica si se deben marcar las subtareas en la barra de tareas de resumen. Para las subtareas, el campo Resumen indica si la información de las barras de Gantt de las subtareas se acumulará en la barra de tareas de resumen. Para las tareas de resumen, el campo Resumen El campo indica si la barra de tareas de resumen muestra barras acumuladas. Debe tener el campo Resumen para tareas de resumen establecido en Sí para que cualquier subtarea se acumule en ellas. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | Obtiene o establece el formato en el que se guardará el documento si se utiliza este objeto de opciones de guardado. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Obtiene o establece la fecha desde la que se empieza a renderizar. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | Obtiene o establece el comparador para ordenar tareas en diagramas de Gantt y hojas de tareas. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | Obtiene o establece la condición que se usa para filtrar tareas representadas en diagramas de Gantt, hoja de tareas y uso de tareas. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Obtiene o establece la lista de las instancias del[`TextStyle`](../../aspose.tasks.visualization/textstyle/) class que aparecen en la vista del proyecto. |
| [TiffCompression](../../aspose.tasks.saving/imagesaveoptions/tiffcompression/) { get; set; } | Obtiene o establece el tipo de compresión que se aplicará al guardar las imágenes generadas en formato TIFF. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Obtiene o establece el[`Timescale`](../saveoptions/timescale/) valor que se usa para controlar cómo se representa la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Obtiene o establece un valor que indica si se debe usar el pincel de degradado al representar el diagrama de Gantt. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/imagesaveoptions/useprojectdefaultfont/) { get; set; } | Obtiene o establece un valor que indica si se debe utilizar la fuente predeterminada para la representación. |
| [VerticalResolution](../../aspose.tasks.saving/imagesaveoptions/verticalresolution/) { get; set; } | Obtiene o establece la resolución vertical en dpi. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Obtiene o establece una lista de las columnas de vista para representar ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). Si no se establece, solo se representan los ID de tarea, los nombres de tarea, el inicio y el final. Si tanto Ver como[`ViewSettings`](../saveoptions/viewsettings/)las propiedades están configuradas, las columnas de View reemplazan las columnas de ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Obtiene o establece una vista ([`View`](../saveoptions/view/) ) para renderizar. Puede usar estas opciones para especificar explícitamente qué vista debe guardarse en formato PDF, HTML o de imagen. Si se establece esta propiedad,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) La propiedad se ignora cuando se guarda el proyecto. La vista debe ser desde una de las siguientes pantallas (([`Screen`](../../aspose.tasks/view/screen/) )): (Gantt, Hoja de tareas, Uso de tareas, Hoja de recursos, Uso de recursos) |

### Ver también

* class [SaveOptions](../saveoptions/)
* espacio de nombres [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* asamblea [Aspose.Tasks](../../)


