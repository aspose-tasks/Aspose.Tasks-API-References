---
title: "CustomProjectPropertyCollection"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une collection de propriétés personnalisées du projet."
type: docs
weight: 61
url: /fr/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

Représente une collection de propriétés personnalisées du projet.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | Initialise une nouvelle instance de la classe [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Crée une nouvelle propriété personnalisée. |
| [add(String name, double value)](#add-java.lang.String-double-) | Crée une nouvelle propriété personnalisée. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Crée une nouvelle propriété personnalisée. |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | Crée une nouvelle propriété personnalisée. |
| [clear()](#clear--) | Efface le PropertyCollection. |
| [isReadOnly()](#isReadOnly--) | Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false. |
| [remove(String name)](#remove-java.lang.String-) | Supprime une propriété avec le nom spécifié de la collection. |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


Initialise une nouvelle instance de la classe [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection).

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


Crée une nouvelle propriété personnalisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété. |
| valeur | booléen | La valeur de l'objet propriété nouvellement créé. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


Crée une nouvelle propriété personnalisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété. |
| valeur | double | La valeur de l'objet propriété nouvellement créé. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


Crée une nouvelle propriété personnalisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété. |
| valeur | java.lang.String | La valeur de l'objet propriété nouvellement créé. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


Crée une nouvelle propriété personnalisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété. |
| valeur | java.util.Date | La valeur de l'objet propriété nouvellement créé. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


Efface le PropertyCollection.

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false.

**Returns:**
boolean - une valeur indiquant si cette collection est en lecture seule ; sinon, false.
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


Supprime une propriété avec le nom spécifié de la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la propriété insensible à la casse. |

**Returns:**
boolean - True si l'élément est trouvé et supprimé avec succès ; sinon, false.
