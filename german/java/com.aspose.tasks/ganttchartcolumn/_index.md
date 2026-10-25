---
title: "GanttChartColumn"
second_title: "Aspose.Tasks for Java API Reference"
description: "Projektansicht‑Klasse"
type: docs
weight: 111
url: /de/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

Projekt‑Ansichtsklasse
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | Initialisiert eine neue Instanz der GanttChartColumn Klasse. |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | Initialisiert eine neue Instanz der GanttChartColumn Klasse. |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | Initialisiert eine neue Instanz der GanttChartColumn Klasse. |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | Initialisiert eine neue Instanz der GanttChartColumn Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | Konvertiert die aktuelle Aufgabe in den Spaltentext. |
| [getField()](#getField--) | Gibt das Spaltenfeld zurück. |
| [setField(int value)](#setField-int-) | Setzt das Spaltenfeld. |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


Initialisiert eine neue Instanz der GanttChartColumn Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Name der Spalte. |
| width | int | Breite der Spalte in Pixeln. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Aufgabendaten‑zu‑Spaltentext‑Konverter. |
| field | int | Spaltenfeld. |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


Initialisiert eine neue Instanz der GanttChartColumn Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Name der Spalte. |
| width | int | Breite der Spalte in Pixeln. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Aufgabendaten‑zu‑Spaltentext‑Konverter. |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


Initialisiert eine neue Instanz der GanttChartColumn Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| width | int | Spaltenbreite in Pixeln. |
| field | int | Spaltenfeld. |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


Initialisiert eine neue Instanz der GanttChartColumn Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Spaltenname. |
| width | int | Spaltenbreite in Pixeln. |
| field | int | Spaltenfeld. |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


Konvertiert die aktuelle Aufgabe in den Spaltentext.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Aktuelle Aufgabe. |

**Returns:**
java.lang.String - Der Spaltentext.
### getField() {#getField--}
```
public int getField()
```


Gibt das Spaltenfeld zurück. `Field`.

**Returns:**
int - Wert des Spaltenfelds.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Setzt das Spaltenfeld.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Wert des Spaltenfelds. |

