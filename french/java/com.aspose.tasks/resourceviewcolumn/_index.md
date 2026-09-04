---
title: "ResourceViewColumn"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Classe de vue des projets utilisée dans les vues ResourceUsage et ResourceSheet."
type: docs
weight: 261
url: /fr/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

Classe de vue du projet utilisée dans la vue ResourceUsage et la vue ResourceSheet.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | Initialise une nouvelle instance de la classe [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | Initialise une nouvelle instance de la classe [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | Initialise une nouvelle instance de la classe [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | Convertit la ressource actuelle en texte de colonne. |
| [getField()](#getField--) | Renvoie le champ de colonne. |
| [setField(int value)](#setField-int-) | Définit le champ de colonne. |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


Initialise une nouvelle instance de la classe [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Nom de la colonne. |
| width | int | Largeur de la colonne en pixels. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Convertisseur de données de ressource en texte de colonne. |
| champ | int | Champ de colonne. |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


Initialise une nouvelle instance de la classe [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Nom de la colonne. |
| width | int | Largeur de la colonne en pixels. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Convertisseur de données de ressource en texte de colonne. |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


Initialise une nouvelle instance de la classe [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| width | int | Largeur de colonne en pixels. |
| champ | int | Champ de colonne. |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


Convertit la ressource actuelle en texte de colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | Ressource actuelle. |

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

