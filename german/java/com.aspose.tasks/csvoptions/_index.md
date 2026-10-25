---
title: "CsvOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben zusätzlicher Optionen beim Speichern eines Projekts als CSV."
type: docs
weight: 56
url: /de/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

Ermöglicht das Angeben zusätzlicher Optionen beim Speichern eines Projekts als CSV.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | Initialisiert eine neue Instanz der [CsvOptions](../../com.aspose/tasks/csvoptions)-Klasse, die verwendet werden kann, um ein Projekt im CSV-Format zu speichern. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | Ruft eine Datenkategorie ab, die gespeichert werden soll. |
| [getEncoding()](#getEncoding--) | Ruft eine Kodierung ab, mit der CSV gespeichert wird. |
| [getIncludeHeaders()](#getIncludeHeaders--) | Ruft einen Wert ab, der angibt, ob Header einbezogen werden sollen oder nicht (Standardwert ist TRUE). |
| [getTextDelimiter()](#getTextDelimiter--) | Ruft ein Texttrennzeichen ab. |
| [getView()](#getView--) | Ruft eine Liste der Ansichtsspalten ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) ab, die im XLSX-Format gespeichert werden sollen. |
| [setDataCategory(int value)](#setDataCategory-int-) | Legt eine Datenkategorie fest, die gespeichert werden soll. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Legt eine Kodierung fest, mit der CSV gespeichert wird. |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | Legt einen Wert fest, der angibt, ob Header einbezogen werden sollen oder nicht (Standardwert ist TRUE). |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | Legt ein Texttrennzeichen fest. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Legt eine Liste der Ansichtsspalten ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) fest, die im XLSX-Format gespeichert werden sollen. |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


Initialisiert eine neue Instanz der [CsvOptions](../../com.aspose/tasks/csvoptions)-Klasse, die verwendet werden kann, um ein Projekt im CSV-Format zu speichern.

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


Ruft eine Datenkategorie ab, die gespeichert werden soll.

**Returns:**
int - eine zu speichernde Datenkategorie.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Ruft eine Kodierung ab, mit der CSV gespeichert wird.

**Returns:**
java.nio.charset.Charset - eine Kodierung, mit der CSV gespeichert wird.
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


Ruft einen Wert ab, der angibt, ob Header einbezogen werden sollen oder nicht (Standardwert ist TRUE).

**Returns:**
boolean - ein Wert, der angibt, ob Header einbezogen werden sollen oder nicht (Standardwert ist TRUE).
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


Ruft ein Texttrennzeichen ab.

**Returns:**
int - ein Texttrennzeichen.
### getView() {#getView--}
```
public final ProjectView getView()
```


Liefert eine Liste der Ansichtsspalten ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)), die im XLSX-Format gespeichert werden sollen. Wenn nicht festgelegt, werden die Standardspalten gespeichert.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


Legt eine Datenkategorie fest, die gespeichert werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine zu speichernde Datenkategorie. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Legt eine Kodierung fest, mit der CSV gespeichert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.nio.charset.Charset | eine Kodierung, mit der CSV gespeichert wird. |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


Legt einen Wert fest, der angibt, ob Header einbezogen werden sollen oder nicht (Standardwert ist TRUE).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Header einbezogen werden sollen oder nicht (Standardwert ist TRUE). |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


Legt ein Texttrennzeichen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Texttrennzeichen. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Setzt eine Liste der Ansichtsspalten ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)), die im XLSX-Format gespeichert werden sollen. Wenn nicht festgelegt, werden die Standardspalten gespeichert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | eine Liste der Ansichtsspalten ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)), die im XLSX-Format gespeichert werden sollen. |

