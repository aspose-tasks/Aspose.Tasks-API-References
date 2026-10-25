---
title: "FilterCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Enthält eine Liste von  Objekten."
type: docs
weight: 92
url: /de/java/com.aspose.tasks/filtercollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class FilterCollection extends AbstractCollection<Filter>
```

Enthält eine Liste von [Filter](../../com.aspose.tasks/filter)-Objekten. Implementiert die ICollection&lt;Filter&gt;-Schnittstelle.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Filter item)](#add-com.aspose.tasks.Filter-) |  |
| [clear()](#clear--) | Entfernt alle Elemente aus dieser Sammlung (optionale Operation). |
| [contains(Filter item)](#contains-com.aspose.tasks.Filter-) | Gibt true zurück, wenn diese Sammlung das angegebene Element enthält. |
| [copyTo(Filter[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Filter---int-) | Kopiert die Elemente aus dem angegebenen Array in diese Sammlung, beginnend ab dem angegebenen Index. |
| [iterator()](#iterator--) | Gibt einen Iterator über die in dieser Sammlung enthaltenen Elemente zurück. |
| [remove(Filter item)](#remove-com.aspose.tasks.Filter-) | Entfernt das angegebene Element aus dieser Sammlung. |
| [size()](#size--) | Ermittelt die Anzahl der in dieser Sammlung enthaltenen Elemente. |
| [toList()](#toList--) | Konvertiert eine Filtersammlung in eine Liste von `Filter`-Objekten. |
### add(Filter item) {#add-com.aspose.tasks.Filter-}
```
public boolean add(Filter item)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) |  |

**Returns:**
boolean
### clear() {#clear--}
```
public void clear()
```


Entfernt alle Elemente aus dieser Sammlung (optionale Operation).

### contains(Filter item) {#contains-com.aspose.tasks.Filter-}
```
public final boolean contains(Filter item)
```


Gibt true zurück, wenn diese Sammlung das angegebene Element enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | das angegebene Element. |

**Returns:**
boolean - true, wenn die Sammlung das angegebene Element enthält.
### copyTo(Filter[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Filter---int-}
```
public final void copyTo(Filter[] array, int arrayIndex)
```


Kopiert die Elemente aus dem angegebenen Array in diese Sammlung, beginnend ab dem angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| array | [Filter\[\]](../../com.aspose.tasks/filter) | das angegebene eindimensionale Array, in das Elemente kopiert werden sollen |
| arrayIndex | int | der nullbasierte Index des angegebenen Arrays, an dem das Kopieren beginnt. |

### iterator() {#iterator--}
```
public Iterator<Filter> iterator()
```


Gibt einen Iterator über die in dieser Sammlung enthaltenen Elemente zurück.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Filter&gt; – Sammlungsiterator.
### remove(Filter item) {#remove-com.aspose.tasks.Filter-}
```
public final boolean remove(Filter item)
```


Entfernt das angegebene Element aus dieser Sammlung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | das angegebene Element. |

**Returns:**
boolean – true, wenn die Operation erfolgreich war.
### size() {#size--}
```
public final int size()
```


Ermittelt die Anzahl der in dieser Sammlung enthaltenen Elemente.

**Returns:**
int - die Anzahl der in dieser Sammlung enthaltenen Elemente.
### toList() {#toList--}
```
public List<Filter> toList()
```


Konvertiert eine Filtersammlung in eine Liste von `Filter`-Objekten.

**Returns:**
java.util.List&lt;com.aspose.tasks.Filter&gt; – generische Liste von `Filter`-Objekten.
