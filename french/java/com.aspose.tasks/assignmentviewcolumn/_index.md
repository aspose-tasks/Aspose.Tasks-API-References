---
title: "AssignmentViewColumn"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Classe de vue des projets."
type: docs
weight: 19
url: /fr/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

Classe de vue du projet.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | Initialise une nouvelle instance de la classe AssignmentViewColumn. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | Convertit l'affectation de ressource actuelle en texte de colonne. |
| [getField()](#getField--) | Renvoie le champ de colonne. |
| [setField(int value)](#setField-int-) | Définit le champ de colonne. |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


Initialise une nouvelle instance de la classe AssignmentViewColumn.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Nom de la colonne. |
| width | int | Largeur de la colonne en pixels. |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | Convertisseur de données d'affectation en texte de colonne. |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


Convertit l'affectation de ressource actuelle en texte de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Affectation actuelle. |

**Returns:**
java.lang.String - Le texte de la colonne.
### getField() {#getField--}
```
public int getField()
```


Renvoie le champ de colonne. `Field`.

**Returns:**
int - valeur du champ de colonne.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Définit le champ de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | valeur du champ de colonne. |

