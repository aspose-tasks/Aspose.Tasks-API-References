---
title: "CsvOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange ytterligare alternativ när projektet sparas till CSV."
type: docs
weight: 56
url: /sv/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

Tillåter att ange ytterligare alternativ när projektet sparas till CSV.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | Initierar en ny instans av klassen [CsvOptions](../../com.aspose/tasks/csvoptions) som kan användas för att spara projekt i CSV-format. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | Hämtar en datakategori som ska sparas. |
| [getEncoding()](#getEncoding--) | Hämtar en kodning för att spara CSV med. |
| [getIncludeHeaders()](#getIncludeHeaders--) | Hämtar ett värde som indikerar om rubriker ska inkluderas eller inte (standardvärdet är TRUE). |
| [getTextDelimiter()](#getTextDelimiter--) | Hämtar en textavgränsare. |
| [getView()](#getView--) | Hämtar en lista över visningskolumnerna ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) för att spara i XLSX-format. |
| [setDataCategory(int value)](#setDataCategory-int-) | Ställer in en datakategori som ska sparas. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ställer in en kodning för att spara CSV med. |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | Ställer in ett värde som indikerar om rubriker ska inkluderas eller inte (standardvärdet är TRUE). |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | Ställer in en textavgränsare. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Ställer in en lista över visningskolumnerna ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) för att spara i XLSX-format. |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


Initierar en ny instans av klassen [CsvOptions](../../com.aspose/tasks/csvoptions) som kan användas för att spara projekt i CSV-format.

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


Hämtar en datakategori som ska sparas.

**Returns:**
int - en datakategori som ska sparas.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Hämtar en kodning för att spara CSV med.

**Returns:**
java.nio.charset.Charset - en kodning för att spara CSV med.
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


Hämtar ett värde som indikerar om rubriker ska inkluderas eller inte (standardvärdet är TRUE).

**Returns:**
boolean - ett värde som indikerar om rubriker ska inkluderas eller inte (standardvärdet är TRUE).
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


Hämtar en textavgränsare.

**Returns:**
int - en textavgränsare.
### getView() {#getView--}
```
public final ProjectView getView()
```


Hämtar en lista över visningskolumnerna ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) för att spara i XLSX-format. Om den inte är inställd sparas standardkolumnerna.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


Ställer in en datakategori som ska sparas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en datakategori som ska sparas. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Ställer in en kodning för att spara CSV med.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.nio.charset.Charset | en kodning för att spara CSV med. |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


Ställer in ett värde som indikerar om rubriker ska inkluderas eller inte (standardvärdet är TRUE).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om rubriker ska inkluderas eller inte (standardvärdet är TRUE). |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


Ställer in en textavgränsare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en textavgränsare. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Ställer in en lista med vykolumnerna ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) att spara i XLSX-format. Om den inte anges sparas standardkolumnerna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | en lista med vykolumnerna ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) att spara i XLSX-format. |

