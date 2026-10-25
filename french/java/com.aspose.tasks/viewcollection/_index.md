---
title: "ViewCollection"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Contient une liste d'objets."
type: docs
weight: 343
url: /fr/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

Contient une liste d'objets [View](../../com.aspose.tasks/view). Étend la classe `AbstractCollection`.
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | Ajoute l'élément spécifié à cette collection. |
| [clear()](#clear--) | Supprime tous les éléments de cette collection. |
| [contains(View item)](#contains-com.aspose.tasks.View-) | Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false. |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié. |
| [getByName(String viewName)](#getByName-java.lang.String-) | Recherche une View par son nom et renvoie la première occurrence dans la collection. |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | Recherche une View avec la propriété Screen spécifiée et renvoie la première occurrence dans la collection. |
| [getParentProject()](#getParentProject--) | Obtient le parent de l'objet View. |
| [iterator()](#iterator--) | Renvoie un itérateur sur les éléments contenus dans cette collection. |
| [remove(View item)](#remove-com.aspose.tasks.View-) | Supprime la première occurrence d'un objet spécifique de cette collection. |
| [size()](#size--) | Obtient le nombre d'éléments contenus dans cette collection. |
| [toList()](#toList--) | Convertit une collection de vues en une liste d'objets [View](../../com.aspose.tasks/view). |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


Ajoute l'élément spécifié à cette collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | l'élément spécifié à ajouter à cette collection. |

**Returns:**
boolean - vrai si l'opération a réussi.
### clear() {#clear--}
```
public final void clear()
```


Supprime tous les éléments de cette collection.

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | l'élément spécifié à rechercher. |

**Returns:**
booléen - true si l'élément spécifié est trouvé dans cette collection ; sinon, false.
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | le tableau unidimensionnel spécifié dans lequel copier les éléments |
| arrayIndex | int | l'index basé sur zéro du tableau spécifié à partir duquel la copie commence. |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


Recherche une View par son nom et renvoie la première occurrence dans la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| viewName | java.lang.String | Nom de la View à rechercher. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


Recherche une View avec la propriété Screen spécifiée et renvoie la première occurrence dans la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| screen | int | Valeur d'énumération [ViewScreen](../../com.aspose.tasks/viewscreen). |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtient le parent de l'objet View. Lecture seule [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


Renvoie un itérateur sur les éléments contenus dans cette collection.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - itérateur de collection.
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


Supprime la première occurrence d'un objet spécifique de cette collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | l'objet spécifié à supprimer. |

**Returns:**
boolean - true si l'objet spécifié a été supprimé avec succès de cette collection ; sinon, false.
### size() {#size--}
```
public final int size()
```


Obtient le nombre d'éléments contenus dans cette collection.

**Returns:**
int - le nombre d'éléments contenus dans cette collection.
### toList() {#toList--}
```
public final List<View> toList()
```


Convertit une collection de vues en une liste d'objets [View](../../com.aspose.tasks/view).

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - Liste générique d'objets [View](../../com.aspose.tasks/view).
