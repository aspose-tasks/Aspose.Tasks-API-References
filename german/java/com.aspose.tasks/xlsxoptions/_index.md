---
title: "XlsxOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Projektseiten zu XLSX."
type: docs
weight: 368
url: /de/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Projektseiten zu XLSX.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | Initialisiert eine neue Instanz der [XlsxOptions](../../com.aspose.tasks/xlsxoptions)-Klasse, die zum Speichern des Projekts im XLSX-Format verwendet werden kann. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Ermittelt eine Liste der Auftragsansichtsspalten, die gerendert werden sollen ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | Ermittelt die Kodierung der resultierenden XLSX-Datei. |
| [getResourceView()](#getResourceView--) | Ermittelt eine Liste der Ressourcensichtsspalten, die gerendert werden sollen ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | Ruft eine Liste der Ansichtsspalten ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) ab, die im XLSX-Format gespeichert werden sollen. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Legt eine Liste der Auftragsansichtsspalten fest, die gerendert werden sollen ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Legt die Kodierung der resultierenden XLSX-Datei fest. |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Legt eine Liste der Ressourcensichtsspalten fest, die gerendert werden sollen ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Legt eine Liste der Ansichtsspalten ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) fest, die im XLSX-Format gespeichert werden sollen. |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


Initialisiert eine neue Instanz der [XlsxOptions](../../com.aspose.tasks/xlsxoptions)-Klasse, die zum Speichern des Projekts im XLSX-Format verwendet werden kann.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Ermittelt eine Liste der Auftragsansichtsspalten, die gerendert werden sollen ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Ermittelt die Kodierung der resultierenden XLSX-Datei. Der Standardwert ist java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Returns:**
java.nio.charset.Charset – die Kodierung der resultierenden XLSX-Datei.
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


Ermittelt eine Liste der Ressourcensichtsspalten, die gerendert werden sollen ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


Liefert eine Liste der Ansichtsspalten ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)), die im XLSX-Format gespeichert werden sollen. Wenn nicht festgelegt, werden die Standardspalten gespeichert.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Legt eine Liste der Auftragsansichtsspalten fest, die gerendert werden sollen ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | eine Liste der Auftragsansichtsspalten, die gerendert werden sollen ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Legt die Kodierung der resultierenden XLSX-Datei fest. Der Standardwert ist java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.nio.charset.Charset | die Kodierung der resultierenden XLSX-Datei. |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


Legt eine Liste der Ressourcensichtsspalten fest, die gerendert werden sollen ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | eine Liste der Ressourcensichtsspalten, die gerendert werden sollen ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Setzt eine Liste der Ansichtsspalten ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)), die im XLSX-Format gespeichert werden sollen. Wenn nicht festgelegt, werden die Standardspalten gespeichert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | eine Liste der Ansichtsspalten ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)), die im XLSX-Format gespeichert werden sollen. |

