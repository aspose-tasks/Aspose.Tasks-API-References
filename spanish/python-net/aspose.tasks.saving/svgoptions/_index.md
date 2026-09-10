---
title: "SvgOptions"
second_title: "Referencia de API de Aspose.Tasks para Python vía .NET"
description: 
type: docs
weight: 170
url: /es/python-net/aspose.tasks.saving/svgoptions/
---

## SvgOptions class

Permite especificar opciones adicionales al renderizar las páginas del proyecto en SVG.

El tipo SvgOptions expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| SvgOptions() | Inicializa una nueva instancia de la clase [SvgOptions](/tasks/python-net/aspose.tasks.saving/svgoptions/) que se puede usar para guardar el proyecto en formato SVG. |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| save_format |  |
| bar_styles | Obtiene o establece la lista de instancias de la clase [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) que aparecen en la vista del proyecto. |
| draw_non_working_time | Obtiene o establece un valor que indica si se debe dibujar el tiempo no laborable (El valor predeterminado es TRUE). |
| end_date | Obtiene o establece una fecha hasta la cual finalizar la renderización. |
| timescale_fit_behavior | Obtiene o establece un comportamiento que define cómo alinear el extremo derecho de la escala de tiempo con el final de la página. |
| fit_content | Obtiene o establece un valor que indica si la altura de la fila debe incrementarse para ajustarse a su contenido. |
| gridlines | Obtiene o establece una lista de [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) que aparecen en la vista del proyecto. |
| legend_drawing_options | Obtiene o establece un valor que define cómo renderizar una leyenda. El valor predeterminado es LegendDrawingOptions.OnEveryPage. |
| legend_items | Obtiene o establece una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de la página.<br/>            Si es nulo, se renderizan los elementos predeterminados. |
| mark_critical_tasks | Obtiene o establece un valor que indica si las tareas críticas deben mostrarse en color rojo (El valor predeterminado es FALSE). |
| non_working_time_color | Obtiene o establece el color del tiempo no laborable. |
| page_count | Obtiene o establece el número de páginas del proyecto. |
| page_size | Obtiene o establece el tamaño de página que se renderizará (El valor predeterminado es PageSize.A4). |
| is_portrait | Obtiene o establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal. |
| presentation_format | Obtiene o establece el [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/) en el que se guardará el documento. |
| roll_up_gantt_bars | Obtiene o establece un valor que indica si las subtareas en la barra de tarea resumida deben marcarse.<br/>            Para las subtareas, el campo Rollup indica si la información de las barras Gantt de la subtarea se consolidará en la barra de tarea resumida.<br/>            Para las tareas resumidas, el campo Rollup indica si la barra de tarea resumida muestra barras consolidadas.<br/>            Debe tener el campo Rollup para tareas resumidas configurado en Yes para que cualquier subtarea se consolide en ellas. |
| start_date | Obtiene o establece la fecha a partir de la cual iniciar la renderización. |
| text_styles | Obtiene o establece la lista de estilos de texto que se aplican durante la renderización de una vista del proyecto. |
| timescale | Obtiene o establece el valor del [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) que se utiliza para controlar cómo se renderiza la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico. |
| use_gradient_brush | Determina si se debe usar un pincel de degradado al renderizar el diseño del proyecto. |
| view | Obtiene o establece una lista de las columnas de vista a renderizar ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            Si no se establece, solo se renderizan los IDs de tarea, nombres de tarea, inicio y fin.<br/>            Si tanto la propiedad View como la de [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) están configuradas, las columnas de View sobrescriben a las columnas de ViewSettings. |
| view_settings | Obtiene o establece una vista ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) para renderizar. Puede usar esta opción para especificar explícitamente qué vista debe guardarse en formatos PDF, HTML o Imagen.<br/>            Si esta propiedad está configurada, la propiedad [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) se ignora cuando se guarda el proyecto.<br/>            La vista debe provenir de una de las siguientes pantallas (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | Obtiene o establece el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada). |
| render_to_single_page | Obtiene o establece un valor que indica si un proyecto debe renderizarse en una sola página<br/>            cuando el proyecto se guarda en formato gráfico.<br/>            El tamaño de página se cambiará para que el proyecto renderizado pueda ajustarse en una sola página. |
| page_saving_callback | Obtiene o establece una devolución de llamada de implementación definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |

### Ver también

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

