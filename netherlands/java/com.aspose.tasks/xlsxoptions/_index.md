---
title: "XlsxOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt toe om extra opties op te geven bij het renderen van projectpagina's naar XLSX."
type: docs
weight: 368
url: /nl/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

Stelt toe om extra opties op te geven bij het renderen van projectpagina's naar XLSX.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | Initialiseert een nieuw exemplaar van de [XlsxOptions](../../com.aspose.tasks/xlsxoptions) klasse die kan worden gebruikt om een project op te slaan in XLSX-formaat. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Haalt een lijst op van de assignments view columns om te renderen ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | Haalt de codering op van het resulterende XLSX-bestand. |
| [getResourceView()](#getResourceView--) | Haalt een lijst op van de resource view columns om te renderen ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | Haalt een lijst van de weergavekolommen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) op om op te slaan in XLSX-formaat. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Stelt een lijst in van de assignments view columns om te renderen ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Stelt de codering in van het resulterende XLSX-bestand. |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Stelt een lijst in van de resource view columns om te renderen ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Stelt een lijst van de weergavekolommen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) in om op te slaan in XLSX-formaat. |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


Initialiseert een nieuw exemplaar van de [XlsxOptions](../../com.aspose.tasks/xlsxoptions) klasse die kan worden gebruikt om een project op te slaan in XLSX-formaat.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Haalt een lijst op van de assignments view columns om te renderen ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Haalt de codering op van het resulterende XLSX-bestand. De standaardwaarde is java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Returns:**
java.nio.charset.Charset - de codering van het resulterende XLSX-bestand.
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


Haalt een lijst op van de resource view columns om te renderen ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


Haalt een lijst van de weergavekolommen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) op om op te slaan in XLSX-formaat. Als deze niet is ingesteld, worden de standaardkolommen opgeslagen.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Stelt een lijst in van de assignments view columns om te renderen ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | een lijst van de assignments view columns om te renderen ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Stelt de codering in van het resulterende XLSX-bestand. De standaardwaarde is java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.nio.charset.Charset | de codering van het resulterende XLSX-bestand. |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


Stelt een lijst in van de resource view columns om te renderen ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | een lijst van de resource view columns om te renderen ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Stelt een lijst van de weergavekolommen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) in om op te slaan in XLSX-formaat. Als deze niet is ingesteld, worden de standaardkolommen opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | een lijst van de weergavekolommen ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) om op te slaan in XLSX-formaat. |

