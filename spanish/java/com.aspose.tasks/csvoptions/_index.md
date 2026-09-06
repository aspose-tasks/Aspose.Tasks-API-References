---
title: "CsvOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar opciones adicionales al guardar el proyecto en CSV."
type: docs
weight: 56
url: /es/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

Permite especificar opciones adicionales al guardar el proyecto en CSV.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | Inicializa una nueva instancia de la clase [CsvOptions](../../com.aspose/tasks/csvoptions) que puede usarse para guardar el proyecto en formato CSV. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | Obtiene una categoría de datos para guardar. |
| [getEncoding()](#getEncoding--) | Obtiene una codificación con la que guardar CSV. |
| [getIncludeHeaders()](#getIncludeHeaders--) | Obtiene un valor que indica si incluir encabezados o no (el valor predeterminado es TRUE). |
| [getTextDelimiter()](#getTextDelimiter--) | Obtiene un delimitador de texto. |
| [getView()](#getView--) | Obtiene una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar en formato XLSX. |
| [setDataCategory(int value)](#setDataCategory-int-) | Establece una categoría de datos para guardar. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Establece una codificación con la que guardar CSV. |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | Establece un valor que indica si incluir encabezados o no (el valor predeterminado es TRUE). |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | Establece un delimitador de texto. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Establece una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar en formato XLSX. |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


Inicializa una nueva instancia de la clase [CsvOptions](../../com.aspose/tasks/csvoptions) que puede usarse para guardar el proyecto en formato CSV.

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


Obtiene una categoría de datos para guardar.

**Returns:**
int - una categoría de datos para guardar.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Obtiene una codificación con la que guardar CSV.

**Returns:**
java.nio.charset.Charset - una codificación con la que guardar CSV.
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


Obtiene un valor que indica si incluir encabezados o no (el valor predeterminado es TRUE).

**Returns:**
boolean - un valor que indica si incluir encabezados o no (el valor predeterminado es TRUE).
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


Obtiene un delimitador de texto.

**Returns:**
int - un delimitador de texto.
### getView() {#getView--}
```
public final ProjectView getView()
```


Obtiene una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar en formato XLSX. Si no se establece, se guardan las columnas predeterminadas.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


Establece una categoría de datos para guardar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | una categoría de datos para guardar. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Establece una codificación con la que guardar CSV.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.nio.charset.Charset | una codificación con la que guardar CSV. |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


Establece un valor que indica si incluir encabezados o no (el valor predeterminado es TRUE).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si incluir encabezados o no (el valor predeterminado es TRUE). |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


Establece un delimitador de texto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un delimitador de texto. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Establece una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar en formato XLSX. Si no se establece, se guardan las columnas predeterminadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | una lista de las columnas de vista ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) para guardar en formato XLSX. |

