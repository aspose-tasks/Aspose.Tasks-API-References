---
title: "AssignmentViewColumn"
second_title: "Aspose.Tasks for Java API-referens"
description: "Klassen för projektvyn."
type: docs
weight: 19
url: /sv/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

Projektets vyklass.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | Initierar en ny instans av klassen AssignmentViewColumn. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | Konverterar aktuell resursallokering till kolumntexten. |
| [getField()](#getField--) | Returnerar kolumnfältet. |
| [setField(int value)](#setField-int-) | Ställer in kolumnfältet. |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


Initierar en ny instans av klassen AssignmentViewColumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Kolumnens namn. |
| width | int | Kolumnens bredd i pixlar. |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | Konverterare för tilldelningsdata till kolumntext. |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


Konverterar aktuell resursallokering till kolumntexten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Aktuell tilldelning. |

**Returns:**
java.lang.String - Kolumntexten.
### getField() {#getField--}
```
public int getField()
```


Returnerar kolumnfältet. `Field`.

**Returns:**
int - kolumnfältets värde.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Ställer in kolumnfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | kolumnfältets värde. |

