---
title: "CsvOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe extra opties op te geven bij het opslaan van een project naar CSV."
type: docs
weight: 56
url: /nl/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

Staat toe extra opties op te geven bij het opslaan van een project naar CSV.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | Initialiseert een nieuw exemplaar van de [CsvOptions](../../com.aspose/tasks/csvoptions) klasse die kan worden gebruikt om een project op te slaan in CSV-formaat. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | Haalt een gegevenscategorie op die moet worden opgeslagen. |
| [getEncoding()](#getEncoding--) | Haalt een codering op om CSV mee op te slaan. |
| [getIncludeHeaders()](#getIncludeHeaders--) | Haalt een waarde op die aangeeft of kopteksten moeten worden opgenomen of niet (standaardwaarde is TRUE). |
| [getTextDelimiter()](#getTextDelimiter--) | Haalt een tekstscheidingsteken op. |
| [getView()](#getView--) | Haalt een lijst van de weergavekolommen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) op om op te slaan in XLSX-formaat. |
| [setDataCategory(int value)](#setDataCategory-int-) | Stelt een gegevenscategorie in die moet worden opgeslagen. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Stelt een codering in om CSV mee op te slaan. |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | Stelt een waarde in die aangeeft of kopteksten moeten worden opgenomen of niet (standaardwaarde is TRUE). |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | Stelt een tekstscheidingsteken in. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Stelt een lijst van de weergavekolommen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) in om op te slaan in XLSX-formaat. |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


Initialiseert een nieuw exemplaar van de [CsvOptions](../../com.aspose/tasks/csvoptions) klasse die kan worden gebruikt om een project op te slaan in CSV-formaat.

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


Haalt een gegevenscategorie op die moet worden opgeslagen.

**Returns:**
int - een gegevenscategorie die moet worden opgeslagen.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Haalt een codering op om CSV mee op te slaan.

**Returns:**
java.nio.charset.Charset - een codering om CSV mee op te slaan.
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


Haalt een waarde op die aangeeft of kopteksten moeten worden opgenomen of niet (standaardwaarde is TRUE).

**Returns:**
boolean - een waarde die aangeeft of kopteksten moeten worden opgenomen of niet (standaardwaarde is TRUE).
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


Haalt een tekstscheidingsteken op.

**Returns:**
int - een tekstscheidingsteken.
### getView() {#getView--}
```
public final ProjectView getView()
```


Haalt een lijst van de weergavekolommen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) op om op te slaan in XLSX-formaat. Als deze niet is ingesteld, worden de standaardkolommen opgeslagen.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


Stelt een gegevenscategorie in die moet worden opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een gegevenscategorie die moet worden opgeslagen. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Stelt een codering in om CSV mee op te slaan.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.nio.charset.Charset | een codering om CSV mee op te slaan. |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


Stelt een waarde in die aangeeft of kopteksten moeten worden opgenomen of niet (standaardwaarde is TRUE).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of kopteksten moeten worden opgenomen of niet (standaardwaarde is TRUE). |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


Stelt een tekstscheidingsteken in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een tekstscheidingsteken. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Stelt een lijst van de weergavekolommen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) in om op te slaan in XLSX-formaat. Als deze niet is ingesteld, worden de standaardkolommen opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | een lijst van de weergavekolommen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) om op te slaan in XLSX-formaat. |

