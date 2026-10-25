---
title: "AssignmentViewColumn"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Klasse voor weergave van projecten."
type: docs
weight: 19
url: /nl/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

Klasse voor projectweergave.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | Initialiseert een nieuw exemplaar van de AssignmentViewColumn-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | Converteert de huidige resource‑toewijzing naar de kolomtekst. |
| [getField()](#getField--) | Retourneert kolomveld. |
| [setField(int value)](#setField-int-) | Stelt kolomveld in. |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


Initialiseert een nieuw exemplaar van de AssignmentViewColumn-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | Naam van de kolom. |
| breedte | int | Breedte van de kolom in pixels. |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | Toewijzingsgegevens naar kolomtekstconverter. |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


Converteert de huidige resource‑toewijzing naar de kolomtekst.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Huidige toewijzing. |

**Returns:**
java.lang.String - De kolomtekst.
### getField() {#getField--}
```
public int getField()
```


Retourneert kolomveld. `Field`.

**Returns:**
int - kolomveldwaarde.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Stelt kolomveld in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | kolomveldwaarde. |

