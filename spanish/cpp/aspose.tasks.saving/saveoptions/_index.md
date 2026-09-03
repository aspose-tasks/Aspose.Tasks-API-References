---
title: "Aspose::Tasks::Saving::SaveOptions class"
linktitle: "SaveOptions"
articleTitle: "SaveOptions"
second_title: "Aspose.Tasks for C++"
description: "Esta es una clase base abstracta para clases que permiten al usuario especificar opciones adicionales al guardar un proyecto en un formato particular."
type: docs
weight: 10
url: /es/cpp/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

**Inherits:** Aspose::Tasks::Saving::SimpleSaveOptions

Esta es una clase base abstracta para clases que permiten al usuario especificar opciones adicionales al guardar un proyecto en un formato particular.

Una instancia de cualquier clase derivada de la clase SaveOptions se pasa a las sobrecargas de Save de tipo stream o string para que el usuario defina opciones personalizadas al guardar un documento.

## Métodos

| Nombre | Descripción |
| --- | --- |
| [get_BarStyles](./get_barstyles/) | Obtiene la lista de las instancias de la clase BarStyle que aparecen en la vista del proyecto. |
| [get_CustomPageSize](./get_custompagesize/) | Obtiene el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada). |
| [get_DrawNonWorkingTime](./get_drawnonworkingtime/) | Obtiene un valor que indica si el tiempo no laborable debe dibujarse (El valor predeterminado es TRUE). |
| [get_EndDate](./get_enddate/) | Obtiene una fecha para terminar la renderización. |
| [get_FitContent](./get_fitcontent/) | Obtiene un valor que indica si la altura de la fila debe incrementarse para ajustarse a su contenido. |
| [get_FitTimescaleToEndOfPage](./get_fittimescaletoendofpage/) | Obtiene si una sección de calendario de una vista debe renderizarse hasta el final (lado derecho) de la última página. Si el valor es false, la sección de calendario se renderiza exactamente hasta EndDate, incluso si hay un espacio vacío en una página. |
| [get_Gridlines](./get_gridlines/) | Obtiene una lista de Gridline que aparecen en la vista del proyecto. |
| [get_IsPortrait](./get_isportrait/) | Obtiene un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal. |
| [get_LegendDrawingOptions](./get_legenddrawingoptions/) | Obtiene un valor que define cómo renderizar una leyenda. El valor predeterminado es LegendDrawingOptions.OnEveryPage. |
| [get_LegendItems](./get_legenditems/) | Obtiene una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de la página. Si es null, se renderizan los elementos predeterminados. |
| [get_MarkCriticalTasks](./get_markcriticaltasks/) | Obtiene un valor que indica si las tareas críticas deben mostrarse en color rojo (El valor predeterminado es FALSE). |
| [get_NonWorkingTimeColor](./get_nonworkingtimecolor/) | Obtiene el color del tiempo no laborable. |
| [get_PageCount](./get_pagecount/) | Obtiene el número de páginas del proyecto. |
| [get_PageSize](./get_pagesize/) | Obtiene el tamaño de página que se renderizará (El valor predeterminado es PageSize.A4). |
| [get_PresentationFormat](./get_presentationformat/) | Obtiene el PresentationFormat en el que se guardará el documento. |
| [get_RenderToSinglePage](./get_rendertosinglepage/) | Obtiene un valor que indica si un proyecto debe renderizarse en una sola página cuando el proyecto se guarda en formato gráfico. El tamaño de página se cambiará para que el proyecto renderizado quepa en una página. |
| [get_RollUpGanttBars](./get_rollupganttbars/) | Obtiene un valor que indica si las subtareas en la barra de tarea resumen deben marcarse. Para las subtareas, el campo Rollup indica si la información de las barras Gantt de la subtarea se consolidará en la barra de tarea resumen. Para las tareas resumen, el campo Rollup indica si la barra de tarea resumen muestra barras consolidadas. Debe tener el campo Rollup de las tareas resumen configurado en Yes para que cualquier subtarea se consolide en ellas. |
| [get_StartDate](./get_startdate/) | Obtiene la fecha desde la cual iniciar la renderización. |
| [get_TextStyles](./get_textstyles/) | Obtiene la lista de estilos de texto que se aplican durante la renderización de una vista de proyecto. |
| [get_Timescale](./get_timescale/) | Obtiene el valor Timescale que se usa para controlar cómo se renderiza la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico. |
| [get_TimescaleFitBehavior](./get_timescalefitbehavior/) | Obtiene un comportamiento que define cómo alinear el extremo derecho de la escala de tiempo con el final de la página. |
| [get_UseGradientBrush](./get_usegradientbrush/) | Obtiene un valor que indica si se debe usar un pincel degradado al renderizar el diagrama de Gantt. |
| [get_View](./get_view/) | Obtiene una lista de las columnas de vista para renderizar ( GanttChartColumn ). Si no se establece, solo se renderizan los IDs de tareas, los nombres de tareas, el inicio y el fin. Si ambas propiedades View y ViewSettings están establecidas, las columnas de View sobrescriben a las columnas de ViewSettings. |
| [get_ViewSettings](./get_viewsettings/) | Obtiene una vista ( View ) para renderizar. Puede usar esta opción para especificar explícitamente qué vista debe guardarse en formatos PDF, HTML o Image. Si esta propiedad está establecida, se ignora la propiedad Visualization::PresentationFormat cuando se guarda el proyecto. La vista debe ser una de las siguientes pantallas (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |
| [set_BarStyles](./set_barstyles/) | Establece la lista de instancias de la clase BarStyle que aparecen en la vista del proyecto. |
| [set_CustomPageSize](./set_custompagesize/) | Establece el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada). |
| [set_DrawNonWorkingTime](./set_drawnonworkingtime/) | Establece un valor que indica si el tiempo no laborable debe dibujarse (el valor predeterminado es TRUE). |
| [set_EndDate](./set_enddate/) | Establece una fecha hasta la cual finalizar la renderización. |
| [set_FitContent](./set_fitcontent/) | Establece un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido. |
| [set_FitTimescaleToEndOfPage](./set_fittimescaletoendofpage/) | Establece si una sección de calendario de una vista debe renderizarse hasta el final (lado derecho) de la última página. Si el valor es false, la sección de calendario se renderiza exactamente hasta EndDate, incluso si hay un espacio vacío en la página. |
| [set_Gridlines](./set_gridlines/) | Establece una lista de Gridline que aparecen en la vista del proyecto. |
| [set_IsPortrait](./set_isportrait/) | Establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal. |
| [set_LegendDrawingOptions](./set_legenddrawingoptions/) | Establece un valor que define cómo renderizar una leyenda. El valor predeterminado es LegendDrawingOptions.OnEveryPage. |
| [set_LegendItems](./set_legenditems/) | Establece una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de la página. Si es null, se renderizan los elementos predeterminados. |
| [set_MarkCriticalTasks](./set_markcriticaltasks/) | Establece un valor que indica si las tareas críticas deben mostrarse en color rojo (el valor predeterminado es FALSE). |
| [set_NonWorkingTimeColor](./set_nonworkingtimecolor/) | Establece el color del tiempo no laborable. |
| [set_PageSize](./set_pagesize/) | Establece el tamaño de página a renderizar (el valor predeterminado es PageSize.A4). |
| [set_PresentationFormat](./set_presentationformat/) | Establece el PresentationFormat en el que se guardará el documento. |
| [set_RenderToSinglePage](./set_rendertosinglepage/) | Establece un valor que indica si un proyecto debe renderizarse en una sola página cuando se guarda en formato gráfico. El tamaño de página se cambiará para que el proyecto renderizado quepa en una página. |
| [set_RollUpGanttBars](./set_rollupganttbars/) | Establece un valor que indica si las subtareas en la barra de tarea resumida deben marcarse. Para las subtareas, el campo Rollup indica si la información de las barras Gantt de la subtarea se consolidará en la barra de tarea resumida. Para las tareas resumidas, el campo Rollup indica si la barra de tarea resumida muestra barras consolidadas. Debe tener el campo Rollup de las tareas resumidas configurado en Yes para que cualquier subtarea se consolide en ellas. |
| [set_StartDate](./set_startdate/) | Establece la fecha a partir de la cual iniciar la renderización. |
| [set_TextStyles](./set_textstyles/) | Establece la lista de estilos de texto que se aplican durante la renderización de una vista del proyecto. |
| [set_Timescale](./set_timescale/) | Establece el valor Timescale que se utiliza para controlar cómo se renderiza la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico. |
| [set_TimescaleFitBehavior](./set_timescalefitbehavior/) | Establece un comportamiento que define cómo alinear el extremo derecho de la escala de tiempo con el final de la página. |
| [set_UseGradientBrush](./set_usegradientbrush/) | Establece un valor que indica si se debe usar un pincel degradado al renderizar el diagrama de Gantt. |
| [set_View](./set_view/) | Establece una lista de las columnas de vista para renderizar ( GanttChartColumn ). Si no se establece, solo se renderizan los IDs de tareas, los nombres de tareas, el inicio y el fin. Si ambas propiedades View y ViewSettings están establecidas, las columnas de View sobrescriben a las columnas de ViewSettings. |
| [set_ViewSettings](./set_viewsettings/) | Establece una vista ( View ) para renderizar. Puede usar esta opción para especificar explícitamente qué vista debe guardarse en formatos PDF, HTML o Image. Si esta propiedad está establecida, se ignora la propiedad Visualization::PresentationFormat cuando se guarda el proyecto. La vista debe ser una de las siguientes pantallas (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

