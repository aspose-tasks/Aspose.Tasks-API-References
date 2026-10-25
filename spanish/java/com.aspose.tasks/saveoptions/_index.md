---
title: "SaveOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Esta es una clase base abstracta para clases que permiten al usuario especificar opciones adicionales al guardar un proyecto en un formato particular."
type: docs
weight: 274
url: /es/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

Esta es una clase base abstracta para clases que permiten al usuario especificar opciones adicionales al guardar un proyecto en un formato particular.

--------------------

Una instancia de cualquier clase derivada de la clase SaveOptions se pasa a las sobrecargas de Save de flujo o Save de cadena para que el usuario defina opciones personalizadas al guardar un documento.
## Métodos

| Método | Descripción |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | Obtiene la lista de las instancias de la clase [BarStyle](../../com.aspose/tasks/barstyle) que aparecen en la vista del proyecto. |
| [getCustomPageSize()](#getCustomPageSize--) | Obtiene el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada). |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | Obtiene un valor que indica si el tiempo no laborable debe dibujarse (El valor predeterminado es TRUE). |
| [getEndDate()](#getEndDate--) | Obtiene una fecha hasta la cual terminar la renderización. |
| [getFitContent()](#getFitContent--) | Obtiene un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido. |
| [getGridlines()](#getGridlines--) | Obtiene una lista de [Gridline](../../com.aspose/tasks/gridline) que aparecen en la vista del proyecto. |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | Obtiene un valor que define cómo renderizar una leyenda. |
| [getLegendItems()](#getLegendItems--) | Obtiene una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de la página. |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | Obtiene un valor que indica si las tareas críticas deben mostrarse en color rojo (El valor predeterminado es FALSE). |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Obtiene el color del tiempo no laborable. |
| [getPageCount()](#getPageCount--) | Obtiene el número de páginas del proyecto. |
| [getPageSize()](#getPageSize--) | Obtiene el tamaño de página a renderizar (El valor predeterminado es PageSize.A4). |
| [getPresentationFormat()](#getPresentationFormat--) | Obtiene el `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) en el que se guardará el documento. |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | Obtiene un valor que indica si un proyecto debe renderizarse en una sola página cuando el proyecto se guarda en formato gráfico. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Obtiene un valor que indica si las subtareas en la barra de tarea resumen deben marcarse. |
| [getStartDate()](#getStartDate--) | Obtiene la fecha a partir de la cual iniciar la renderización. |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | Obtiene una devolución de llamada que puede usarse para personalizar algunos aspectos de la renderización de enlaces de tareas. |
| [getTextStyles()](#getTextStyles--) | Obtiene la lista de estilos de texto que se aplican durante la renderización de una vista de proyecto. |
| [getTimescale()](#getTimescale--) | Obtiene el valor `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) que se usa para controlar cómo se renderiza la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico. |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | Obtiene un comportamiento que define cómo alinear el extremo derecho de la escala de tiempo con el final de la página. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Obtiene un valor que indica si se debe usar un pincel degradado al renderizar el diagrama de Gantt. |
| [getView()](#getView--) | Obtiene una lista de las columnas de vista a renderizar ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | Obtiene una vista (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) para renderizar. |
| [isPortrait()](#isPortrait--) | Obtiene un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal. |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | Establece la lista de instancias de la clase [BarStyle](../../com.aspose.tasks/barstyle) que aparecen en la vista del proyecto. |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | Establece el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada). |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | Establece un valor que indica si el tiempo no laborable debe dibujarse (el valor predeterminado es TRUE). |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Establece una fecha hasta la cual finalizar la renderización. |
| [setFitContent(boolean value)](#setFitContent-boolean-) | Establece un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido. |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | Establece una lista de [Gridline](../../com.aspose.tasks/gridline) que aparecen en la vista del proyecto. |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | Establece un valor que define cómo renderizar una leyenda. |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | Establece una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de la página. |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | Establece un valor que indica si las tareas críticas deben mostrarse en color rojo (el valor predeterminado es FALSE). |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Establece el color del tiempo no laborable. |
| [setPageSize(int value)](#setPageSize-int-) | Establece el tamaño de página a renderizar (el valor predeterminado es PageSize.A4). |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal. |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | Establece el `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) en el que se guardará el documento. |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | Establece un valor que indica si un proyecto debe renderizarse en una sola página cuando el proyecto se guarda en formato gráfico. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Establece un valor que indica si las subtareas en la barra de tarea resumen deben marcarse. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Establece la fecha a partir de la cual iniciar la renderización. |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | Establece una devolución de llamada que puede usarse para personalizar algunos aspectos de la renderización de enlaces de tareas. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Establece la lista de estilos de texto que se aplican durante la renderización de una vista de proyecto. |
| [setTimescale(int value)](#setTimescale-int-) | Establece el valor de `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) que se utiliza para controlar cómo se renderiza la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico. |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | Establece un comportamiento que define cómo alinear el extremo derecho de la escala de tiempo con el final de la página. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Establece un valor que indica si se debe usar un pincel de degradado al renderizar el diagrama de Gantt. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Establece una lista de las columnas de vista a renderizar ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | Establece una vista (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) para renderizar. |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


Obtiene la lista de las instancias de la clase [BarStyle](../../com.aspose/tasks/barstyle) que aparecen en la vista del proyecto.

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - la lista de instancias de la clase [BarStyle](../../com.aspose.tasks/barstyle) que aparecen en la vista del proyecto.
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


Obtiene el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada).

**Returns:**
java.awt.geom.Dimension2D - el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada).
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


Obtiene un valor que indica si el tiempo no laborable debe dibujarse (El valor predeterminado es TRUE).

**Returns:**
boolean - un valor que indica si se debe dibujar el tiempo no laborable (El valor predeterminado es TRUE).
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Obtiene una fecha hasta la cual terminar la renderización.

**Returns:**
java.util.Date - una fecha para terminar la renderización.
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


Obtiene un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido.

**Returns:**
boolean - un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido.
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


Obtiene una lista de [Gridline](../../com.aspose/tasks/gridline) que aparecen en la vista del proyecto.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - una lista de [Gridline](../../com.aspose.tasks/gridline) que aparecen en la vista del proyecto.
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


Obtiene un valor que define cómo renderizar una leyenda. El valor predeterminado es LegendDrawingOptions.OnEveryPage.

Solo es aplicable cuando se renderiza la vista de diagrama de Gantt.

**Returns:**
int - un valor que define cómo renderizar una leyenda.
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


Obtiene una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de página. Si es null, se renderizan los elementos predeterminados.

Solo es aplicable cuando se renderiza la vista de diagrama de Gantt.

**Returns:**
com.aspose.tasks.PageLegendItem[] - una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de página.
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


Obtiene un valor que indica si las tareas críticas deben mostrarse en color rojo (El valor predeterminado es FALSE).

**Returns:**
boolean - un valor que indica si las tareas críticas deben mostrarse en color rojo (El valor predeterminado es FALSE).
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Obtiene el color del tiempo no laborable.

**Returns:**
java.awt.Color - el color del tiempo no laborable.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Obtiene el número de páginas del proyecto.

**Returns:**
int - el número de páginas del proyecto.
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


Obtiene el tamaño de página a renderizar (El valor predeterminado es PageSize.A4).

**Returns:**
int - el tamaño de la página a renderizar (El valor predeterminado es PageSize.A4).
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


Obtiene el `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) en el que se guardará el documento.

**Returns:**
int - el `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) en el que se guardará el documento.
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


Obtiene un valor que indica si un proyecto debe renderizarse en una sola página cuando se guarda el proyecto en formato gráfico. El tamaño de la página se cambiará para que el proyecto renderizado pueda ajustarse a una página.

**Returns:**
boolean - un valor que indica si un proyecto debe renderizarse en una sola página cuando el proyecto se guarda en formato gráfico.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Obtiene un valor que indica si las subtareas en la barra de tarea resumen deben marcarse. Para las subtareas, el campo Rollup indica si la información de las barras Gantt de la subtarea se consolidará en la barra de tarea resumen. Para las tareas resumen, el campo Rollup indica si la barra de tarea resumen muestra barras consolidadas. Debe tener el campo Rollup para tareas resumen configurado en Sí para que cualquier subtarea se consolide en ellas.

--------------------

Solo es aplicable cuando se renderiza la vista de diagrama de Gantt.

**Returns:**
boolean - un valor que indica si las subtareas en la barra de tarea resumen deben marcarse.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Obtiene la fecha a partir de la cual iniciar la renderización.

**Returns:**
java.util.Date - la fecha a partir de la cual comenzar a renderizar.
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


Obtiene una devolución de llamada que puede usarse para personalizar algunos aspectos de la renderización de enlaces de tareas.

Solo es aplicable cuando se renderiza la vista de diagrama de Gantt.

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Obtiene la lista de estilos de texto que se aplican durante la renderización de una vista de proyecto.

--------------------

Estos estilos sobrescriben los estilos definidos con GanttCharView.setTextStyles.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - la lista de estilos de texto que se aplican durante el renderizado de una vista de proyecto.
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


Obtiene el valor `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) que se usa para controlar cómo se renderiza la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico.

**Returns:**
int - el valor `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) que se utiliza para controlar cómo se renderiza la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico.
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


Obtiene un comportamiento que define cómo alinear el extremo derecho de la escala de tiempo con el final de la página.

**Returns:**
int - un comportamiento que define cómo alinear el extremo derecho de la escala de tiempo con el final de la página.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Obtiene un valor que indica si se debe usar un pincel degradado al renderizar el diagrama de Gantt.

--------------------

Solo es aplicable cuando se renderiza la vista de diagrama de Gantt.

**Returns:**
boolean - un valor que indica si se debe usar un pincel degradado al renderizar el diagrama de Gantt.
### getView() {#getView--}
```
public final ProjectView getView()
```


Obtiene una lista de las columnas de vista a renderizar ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Si no se establece, solo se renderizan los IDs de tarea, los nombres de tarea, el inicio y el fin. Si se establecen ambas propiedades View y `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)), las columnas de View sobrescriben a las columnas de ViewSettings.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


Obtiene una vista (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) para renderizar. Puede usar esta opción para especificar explícitamente qué vista debe guardarse en formatos PDF, HTML o Image. Si esta propiedad está establecida, la propiedad [PresentationFormat](../../com.aspose.tasks/presentationformat) se ignora cuando se guarda el proyecto. La vista debe provenir de una de las siguientes pantallas ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Obtiene un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal.

--------------------

No es aplicable cuando SaveOptions.getPageSize() == PageSize.DefinedInView. En este caso se utiliza [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--). No es aplicable cuando se establece [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--).

**Returns:**
boolean - un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal.
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


Establece la lista de instancias de la clase [BarStyle](../../com.aspose.tasks/barstyle) que aparecen en la vista del proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | la lista de instancias de la clase [BarStyle](../../com.aspose.tasks/barstyle) que aparecen en la vista del proyecto. |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


Establece el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.geom.Dimension2D | el tamaño de página personalizado en puntos (1 punto = 1/72 de pulgada). |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


Establece un valor que indica si el tiempo no laborable debe dibujarse (el valor predeterminado es TRUE).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si el tiempo no laborable debe dibujarse (el valor predeterminado es TRUE). |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Establece una fecha hasta la cual finalizar la renderización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | una fecha hasta la cual finalizar el renderizado. |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


Establece un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si la altura de la fila debe aumentarse para ajustarse a su contenido. |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


Establece una lista de [Gridline](../../com.aspose.tasks/gridline) que aparecen en la vista del proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | una lista de [Gridline](../../com.aspose.tasks/gridline) que aparecen en la vista del proyecto. |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


Establece un valor que define cómo renderizar una leyenda. El valor predeterminado es LegendDrawingOptions.OnEveryPage.

Solo es aplicable cuando se renderiza la vista de diagrama de Gantt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un valor que define cómo renderizar una leyenda. |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


Establece una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de página. Si es null, se renderizan los elementos predeterminados.

Solo es aplicable cuando se renderiza la vista de diagrama de Gantt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de página. |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


Establece un valor que indica si las tareas críticas deben mostrarse en color rojo (el valor predeterminado es FALSE).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si las tareas críticas deben mostrarse en color rojo (el valor predeterminado es FALSE). |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Establece el color del tiempo no laborable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color | el color del tiempo no laborable. |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


Establece el tamaño de página a renderizar (el valor predeterminado es PageSize.A4).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el tamaño de la página a renderizar (El valor predeterminado es PageSize.A4). |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal.

--------------------

No es aplicable cuando SaveOptions.PageSize == Visualization.PageSize.DefinedInView. En este caso [PageSettings.setPortrait(boolean)](../../com.aspose/tasks/pagesettings\#setPortrait-boolean-) se usa en su lugar. No es aplicable cuando [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) está configurado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal. |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


Establece el `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) en el que se guardará el documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | int | el `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) en el que se guardará el documento. |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


Establece un valor que indica si un proyecto debe renderizarse en una sola página cuando el proyecto se guarda en formato gráfico. El tamaño de página se cambiará para que el proyecto renderizado quepa en una sola página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si un proyecto debe renderizarse en una sola página cuando el proyecto se guarda en formato gráfico. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Establece un valor que indica si las subtareas en la barra de tarea resumida deben marcarse. Para las subtareas, el campo Rollup indica si la información de las barras Gantt de la subtarea se consolidará en la barra de tarea resumida. Para las tareas resumidas, el campo Rollup indica si la barra de tarea resumida muestra barras consolidadas. Debe tener el campo Rollup para tareas resumidas configurado en Sí para que cualquier subtarea se consolide en ellas.

--------------------

Solo es aplicable cuando se renderiza la vista de diagrama de Gantt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si las subtareas en la barra de tarea resumida deben marcarse. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Establece la fecha a partir de la cual iniciar la renderización.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | la fecha a partir de la cual iniciar la renderización. |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


Establece una devolución de llamada que puede usarse para personalizar algunos aspectos de la renderización de enlaces de tareas.

Solo es aplicable cuando se renderiza la vista de diagrama de Gantt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | una devolución de llamada que puede usarse para personalizar algunos aspectos de la renderización de enlaces de tareas. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Establece la lista de estilos de texto que se aplican durante la renderización de una vista de proyecto.

--------------------

Estos estilos sobrescriben los estilos definidos con GanttCharView.setTextStyles.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | la lista de estilos de texto que se aplican durante la renderización de una vista de proyecto. |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


Establece el valor de `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) que se utiliza para controlar cómo se renderiza la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | int | el valor `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) que se usa para controlar cómo se renderiza la escala de tiempo (si está presente) cuando el proyecto se guarda en formato gráfico. |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


Establece un comportamiento que define cómo alinear el extremo derecho de la escala de tiempo con el final de la página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un comportamiento que define cómo alinear el extremo derecho de la escala de tiempo con el final de la página. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Establece un valor que indica si se debe usar un pincel de degradado al renderizar el diagrama de Gantt.

--------------------

Solo es aplicable cuando se renderiza la vista de diagrama de Gantt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe usar un pincel degradado al renderizar el diagrama de Gantt. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Establece una lista de las columnas de vista a renderizar ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Si no se establece, solo se renderizan los IDs de tarea, los nombres de tarea, el inicio y el fin. Si tanto View como las propiedades `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) están configuradas, las columnas de View sobrescriben a las de ViewSettings.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | una lista de las columnas de vista a renderizar ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


Establece una vista (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) para renderizar. Puede usar esta opción para especificar explícitamente qué vista debe guardarse en formatos PDF, HTML o Imagen. Si esta propiedad está establecida, la propiedad [PresentationFormat](../../com.aspose.tasks/presentationformat) se ignora cuando se guarda el proyecto. La vista debe ser una de las siguientes pantallas ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | una vista (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) para renderizar. |

