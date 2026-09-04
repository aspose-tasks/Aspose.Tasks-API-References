---
title: "RateCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Sammlung dar, die Objekte enthält."
type: docs
weight: 234
url: /de/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

Stellt eine Sammlung dar, die [Rate](../../com.aspose.tasks/rate)-Objekte enthält.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | Fügt dieser Sammlung eine neue [Rate](../../com.aspose.tasks/rate)-Instanz hinzu. |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | Fügt dieser Sammlung eine neue [Rate](../../com.aspose.tasks/rate)-Instanz hinzu. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | Gibt das Element am angegebenen Index zurück. |
| [getParentResource()](#getParentResource--) | Liefert das übergeordnete [Resource](../../com.aspose.tasks/resource)-Objekt für diese Sammlung. |
| [isReadOnly()](#isReadOnly--) | Liefert einen Wert, der angibt, ob diese Sammlung schreibgeschützt ist. |
| [iterator()](#iterator--) | Gibt einen Enumerator für diese Sammlung zurück. |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | Entfernt die Rate-Instanz aus dieser Sammlung. |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | Setzt das Element am angegebenen Index. |
| [size()](#size--) | Liefert die Anzahl der im RateCollection enthaltenen Elemente. |
| [toList()](#toList--) | Konvertiert das [RateCollection](../../com.aspose.tasks/ratecollection)-Objekt in eine Liste von [Rate](../../com.aspose.tasks/rate)-Objekten. |
| [toList(int type)](#toList-int-) | Konvertiert das [RateCollection](../../com.aspose.tasks/ratecollection)-Objekt in eine Liste von [Rate](../../com.aspose.tasks/rate)-Objekten, gefiltert nach dem angegebenen [RateType](../../com.aspose.tasks/ratetype)-Typ. |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


Fügt dieser Sammlung eine neue [Rate](../../com.aspose.tasks/rate)-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ratesFrom | java.util.Date | Das Datum, an dem der neue Satz wirksam wird. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


Fügt dieser Sammlung eine neue [Rate](../../com.aspose.tasks/rate)-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ratesFrom | java.util.Date | Das Datum, an dem der neue Satz wirksam wird. |
| Typ | int | Die Tariftabelle, in die eingefügt werden soll. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### clear() {#clear--}
```
public final void clear()
```




### entrySet() {#entrySet--}
```
public Set<Map.Entry<Integer,RateByDateCollection>> entrySet()
```


(@inheritDoc\}

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;java.lang.Integer,com.aspose.tasks.RateByDateCollection&gt;&gt; - \{@inheritDoc\}
### get(Object key) {#get-java.lang.Object-}
```
public final RateByDateCollection get(Object key)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


Gibt das Element am angegebenen Index zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | int | Der nullbasierte Index des abzurufenden Elements. |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


Liefert das übergeordnete [Resource](../../com.aspose.tasks/resource)-Objekt für diese Sammlung.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Liefert einen Wert, der angibt, ob diese Sammlung schreibgeschützt ist.

**Returns:**
boolean - ein Wert, der angibt, ob diese Sammlung schreibgeschützt ist.
### iterator() {#iterator--}
```
public final Iterator iterator()
```


Gibt einen Enumerator für diese Sammlung zurück.

**Returns:**
java.util.Iterator - ein Enumerator für diese Sammlung.
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


Entfernt die Rate-Instanz aus dieser Sammlung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | Das zu entfernende Element. |

**Returns:**
boolean - true, wenn die angegebene Rate erfolgreich entfernt wurde; andernfalls false.
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


Setzt das Element am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | int | Der nullbasierte Index des zu setzenden Elements. |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | Das Element, das am angegebenen Index gesetzt werden soll. |

### size() {#size--}
```
public final int size()
```


Liefert die Anzahl der im RateCollection enthaltenen Elemente.

**Returns:**
int - die Anzahl der im RateCollection enthaltenen Elemente.
### toList() {#toList--}
```
public final List<Rate> toList()
```


Konvertiert das [RateCollection](../../com.aspose.tasks/ratecollection)-Objekt in eine Liste von [Rate](../../com.aspose.tasks/rate)-Objekten.

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - Liste von [Rate](../../com.aspose.tasks/rate)-Objekten.
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


Konvertiert das [RateCollection](../../com.aspose.tasks/ratecollection)-Objekt in eine Liste von [Rate](../../com.aspose.tasks/rate)-Objekten, gefiltert nach dem angegebenen [RateType](../../com.aspose.tasks/ratetype)-Typ.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | int | Der zu filternde Typ. |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - eine Liste von [Rate](../../com.aspose.tasks/rate)-Objekten.
