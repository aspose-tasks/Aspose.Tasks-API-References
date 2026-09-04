---
title: "ViewCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Enthält eine Liste von  Objekten."
type: docs
weight: 343
url: /de/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

Enthält eine Liste von [View](../../com.aspose.tasks/view) Objekten. Erweitert die Klasse `AbstractCollection`.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | Fügt das angegebene Element zu dieser Sammlung hinzu. |
| [clear()](#clear--) | Entfernt alle Elemente aus dieser Sammlung. |
| [contains(View item)](#contains-com.aspose.tasks.View-) | Gibt true zurück, wenn das angegebene Element in dieser Sammlung gefunden wird; andernfalls false. |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | Kopiert die Elemente dieser Sammlung in das angegebene Array, beginnend beim angegebenen Array-Index. |
| [getByName(String viewName)](#getByName-java.lang.String-) | Sucht nach einer View mit dem Namen und gibt das erste Vorkommen in der Sammlung zurück. |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | Sucht nach einer View mit der angegebenen Screen-Eigenschaft und gibt das erste Vorkommen in der Sammlung zurück. |
| [getParentProject()](#getParentProject--) | Ruft das übergeordnete Element des View-Objekts ab. |
| [iterator()](#iterator--) | Gibt einen Iterator über die in dieser Sammlung enthaltenen Elemente zurück. |
| [remove(View item)](#remove-com.aspose.tasks.View-) | Entfernt das erste Vorkommen eines bestimmten Objekts aus dieser Sammlung. |
| [size()](#size--) | Ermittelt die Anzahl der in dieser Sammlung enthaltenen Elemente. |
| [toList()](#toList--) | Konvertiert eine View-Sammlung in eine Liste von [View](../../com.aspose.tasks/view) Objekten. |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


Fügt das angegebene Element zu dieser Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | das angegebene Element, das zu dieser Sammlung hinzugefügt werden soll. |

**Returns:**
boolean – true, wenn die Operation erfolgreich war.
### clear() {#clear--}
```
public final void clear()
```


Entfernt alle Elemente aus dieser Sammlung.

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


Gibt true zurück, wenn das angegebene Element in dieser Sammlung gefunden wird; andernfalls false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | das angegebene Element zum Suchen. |

**Returns:**
boolean - true, wenn das angegebene Element in dieser Sammlung gefunden wird; andernfalls false.
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


Kopiert die Elemente dieser Sammlung in das angegebene Array, beginnend beim angegebenen Array-Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | das angegebene eindimensionale Array, in das Elemente kopiert werden sollen |
| arrayIndex | int | der nullbasierte Index des angegebenen Arrays, an dem das Kopieren beginnt. |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


Sucht nach einer View mit dem Namen und gibt das erste Vorkommen in der Sammlung zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| viewName | java.lang.String | Name der zu suchenden View. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


Sucht nach einer View mit der angegebenen Screen-Eigenschaft und gibt das erste Vorkommen in der Sammlung zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| screen | int | [ViewScreen](../../com.aspose.tasks/viewscreen) Enumerationswert. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ruft das übergeordnete Element des View-Objekts ab. Nur lesbar [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


Gibt einen Iterator über die in dieser Sammlung enthaltenen Elemente zurück.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; – Sammlungsiterator.
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


Entfernt das erste Vorkommen eines bestimmten Objekts aus dieser Sammlung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | das angegebene Objekt zum Entfernen. |

**Returns:**
boolean - true, wenn das angegebene Objekt erfolgreich aus dieser Sammlung entfernt wurde; andernfalls false.
### size() {#size--}
```
public final int size()
```


Ermittelt die Anzahl der in dieser Sammlung enthaltenen Elemente.

**Returns:**
int - die Anzahl der in dieser Sammlung enthaltenen Elemente.
### toList() {#toList--}
```
public final List<View> toList()
```


Konvertiert eine View-Sammlung in eine Liste von [View](../../com.aspose.tasks/view) Objekten.

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; – Generische Liste von [View](../../com.aspose.tasks/view) Objekten.
