---
title: Class PdfSaveOptions
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Aspose.Tasks.Saving.PdfSaveOptions clase. Permite especificar opciones adicionales al renderizar páginas de proyecto a PDF.
type: docs
weight: 1860
url: /es/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Permite especificar opciones adicionales al renderizar páginas de proyecto a PDF.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Inicializa una nueva instancia del`PdfSaveOptions`clase que se puede utilizar para guardar un documento en el[`PDF`](../savefileformat/) formato. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Obtiene o establece la lista de las instancias del[`BarStyle`](../../aspose.tasks.visualization/barstyle/) class que aparecen en la vista del proyecto. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance/) { get; set; } | Obtiene o establece un nivel de cumplimiento deseado para el documento PDF generado. El valor predeterminado esPdf15 . |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Obtiene o establece el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada). |
| [DefaultFontName](../../aspose.tasks.saving/pdfsaveoptions/defaultfontname/) { get; set; } | Obtiene o establece la fuente predeterminada para renderizar. |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/) { get; set; } | Obtiene o establece los detalles de una firma digital. Si no se establece, no se realizará ninguna firma. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Obtiene o establece un valor que indica si se debe dibujar el tiempo no laborable (el valor predeterminado es VERDADERO). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails/) { get; set; } | Obtiene o establece detalles de cifrado. Si no se establece, no se realizará ningún cifrado. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Obtiene o establece una fecha para terminar de renderizar. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Obtiene o establece un valor que indica si se debe aumentar el alto de la fila para que se ajuste a su contenido. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | Obtiene o establece si una sección de calendario de una vista debe representarse al final (lado derecho) de la última página. Si el valor es falso, la sección de calendario se representa exactamente en EndDate, incluso si hay un espacio vacío en una página. |
| [FontResolveCallback](../../aspose.tasks.saving/pdfsaveoptions/fontresolvecallback/) { get; set; } | Obtiene o establece una devolución de llamada que se puede usar para personalizar las fuentes resueltas. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Obtiene o establece una lista de[`Gridline`](../../aspose.tasks.visualization/gridline/) que aparecen en la vista del proyecto. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | Obtiene o establece un valor que indica si la leyenda debe mostrarse en cada página (el valor predeterminado es VERDADERO). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Obtiene o establece un valor que indica si las tareas críticas deben mostrarse en color rojo (el valor predeterminado es FALSO). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Obtiene o establece el color del tiempo no laborable. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Obtiene o establece el número de páginas del proyecto. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages/) { get; set; } | Obtiene o establece la lista de números de página para guardar al guardar el diseño del proyecto en archivos separados. Todas las páginas se guardarán si esta lista está vacía. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback/) { get; set; } | Obtiene o establece una devolución de llamada definida por el usuario que se usa para obtener un flujo de salida para cada página renderizada. Es aplicable cuando[`SaveToSeparateFiles`](./savetoseparatefiles/) se utiliza la opción. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Obtiene o establece el tamaño de la página que se representará (el valor predeterminado es PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Obtiene o establece el[`PresentationFormat`](../saveoptions/presentationformat/) en el que se guardará el documento. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap/) { get; set; } | Obtiene o establece un valor que indica si se debe reducir un espacio entre la última tarea y el pie de página. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Obtiene o establece un valor que indica si un proyecto debe representarse en una sola página cuando el proyecto se guarda en formato gráfico. El tamaño de la página cambiará para que el proyecto representado pueda caber en una sola página. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Obtiene o establece un valor que indica si se deben marcar las subtareas en la barra de tareas de resumen. Para las subtareas, el campo Resumen indica si la información de las barras de Gantt de las subtareas se acumulará en la barra de tareas de resumen. Para las tareas de resumen, el campo Resumen El campo indica si la barra de tareas de resumen muestra barras acumuladas. Debe tener el campo Resumen para tareas de resumen establecido en Sí para que cualquier subtarea se acumule en ellas. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | Obtiene o establece el formato en el que se guardará el documento si se utiliza este objeto de opciones de guardado. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles/) { get; set; } | Obtiene o establece un valor que indica si se deben guardar las páginas del proyecto en archivos independientes. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Obtiene o establece la fecha desde la que se empieza a renderizar. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | Obtiene o establece el comparador para ordenar tareas en diagramas de Gantt y hojas de tareas. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | Obtiene o establece la condición que se usa para filtrar tareas representadas en diagramas de Gantt, hoja de tareas y uso de tareas. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression/) { get; set; } | Obtiene o establece un tipo de compresión que se usará para todos los flujos de contenido excepto imágenes. El valor predeterminado esFlate . |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Obtiene o establece la lista de las instancias del[`TextStyle`](../../aspose.tasks.visualization/textstyle/) class que aparecen en la vista del proyecto. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Obtiene o establece el[`Timescale`](../saveoptions/timescale/) valor que se usa para controlar cómo se representa la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Obtiene o establece un valor que indica si se debe usar el pincel de degradado al representar el diagrama de Gantt. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont/) { get; set; } | Obtiene o establece un valor que indica si se debe utilizar la fuente predeterminada para la representación. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Obtiene o establece una lista de las columnas de vista para representar ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). Si no se establece, solo se representan los ID de tarea, los nombres de tarea, el inicio y el final. Si tanto Ver como[`ViewSettings`](../saveoptions/viewsettings/)las propiedades están configuradas, las columnas de View reemplazan las columnas de ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Obtiene o establece una vista ([`View`](../saveoptions/view/) ) para renderizar. Puede usar estas opciones para especificar explícitamente qué vista debe guardarse en formato PDF, HTML o de imagen. Si se establece esta propiedad,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) La propiedad se ignora cuando se guarda el proyecto. La vista debe ser desde una de las siguientes pantallas (([`Screen`](../../aspose.tasks/view/screen/) )): (Gantt, Hoja de tareas, Uso de tareas, Hoja de recursos, Uso de recursos) |

### Ver también

* class [SaveOptions](../saveoptions/)
* espacio de nombres [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* asamblea [Aspose.Tasks](../../)


