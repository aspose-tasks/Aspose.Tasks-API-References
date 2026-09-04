---
title: "AssignmentViewColumn"
second_title: "Aspose.Tasks for Java API Reference"
description: "Klasse für die Projektansicht."
type: docs
weight: 19
url: /de/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

Klasse für die Projektansicht.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | Initialisiert eine neue Instanz der Klasse AssignmentViewColumn. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | Konvertiert die aktuelle Ressourcenzuweisung in den Spaltentext. |
| [getField()](#getField--) | Gibt das Spaltenfeld zurück. |
| [setField(int value)](#setField-int-) | Setzt das Spaltenfeld. |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


Initialisiert eine neue Instanz der Klasse AssignmentViewColumn.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Name der Spalte. |
| width | int | Breite der Spalte in Pixeln. |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | Konverter für Zuweisungsdaten zum Spaltentext. |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


Konvertiert die aktuelle Ressourcenzuweisung in den Spaltentext.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Aktuelle Zuweisung. |

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

