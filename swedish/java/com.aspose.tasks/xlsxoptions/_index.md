---
title: "XlsxOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att specificera ytterligare alternativ när projekt sidor renderas till XLSX."
type: docs
weight: 368
url: /sv/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

Tillåter att specificera ytterligare alternativ när projekt sidor renderas till XLSX.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | Initierar en ny instans av klassen [XlsxOptions](../../com.aspose/tasks/xlsxoptions) som kan användas för att spara projekt i XLSX-format. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Hämtar en lista med tilldelningsvy‑kolumner att rendera ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | Hämtar kodningen för den resulterande XLSX-filen. |
| [getResourceView()](#getResourceView--) | Hämtar en lista med resursvy‑kolumner att rendera ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | Hämtar en lista över visningskolumnerna ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) för att spara i XLSX-format. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Ställer in en lista med tilldelningsvy‑kolumner att rendera ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ställer in kodningen för den resulterande XLSX-filen. |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Ställer in en lista med resursvy‑kolumner att rendera ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Ställer in en lista över visningskolumnerna ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) för att spara i XLSX-format. |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


Initierar en ny instans av klassen [XlsxOptions](../../com.aspose/tasks/xlsxoptions) som kan användas för att spara projekt i XLSX-format.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Hämtar en lista med tilldelningsvy‑kolumner att rendera ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Hämtar kodningen för den resulterande XLSX-filen. Standardvärdet är java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Returns:**
java.nio.charset.Charset – kodningen för den resulterande XLSX-filen.
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


Hämtar en lista med resursvy‑kolumner att rendera ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


Hämtar en lista över visningskolumnerna ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) för att spara i XLSX-format. Om den inte är inställd sparas standardkolumnerna.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Ställer in en lista med tilldelningsvy‑kolumner att rendera ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | en lista med tilldelningsvy‑kolumner att rendera ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Ställer in kodningen för den resulterande XLSX-filen. Standardvärdet är java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.nio.charset.Charset | kodningen för den resulterande XLSX-filen. |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


Ställer in en lista med resursvy‑kolumner att rendera ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | en lista med resursvy‑kolumner att rendera ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Ställer in en lista med vykolumnerna ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) att spara i XLSX-format. Om den inte anges sparas standardkolumnerna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | en lista med vykolumnerna ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) att spara i XLSX-format. |

