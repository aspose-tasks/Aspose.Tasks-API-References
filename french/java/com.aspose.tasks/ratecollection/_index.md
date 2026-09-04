---
title: "RateCollection"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une collection qui contient des objets."
type: docs
weight: 234
url: /fr/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

Représente une collection qui contient des objets [Rate](../../com.aspose.tasks/rate).
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | Ajoute une nouvelle instance [Rate](../../com.aspose.tasks/rate) à cette collection. |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | Ajoute une nouvelle instance [Rate](../../com.aspose.tasks/rate) à cette collection. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | Renvoie l'élément à l'index spécifié. |
| [getParentResource()](#getParentResource--) | Obtient l'objet parent [Resource](../../com.aspose.tasks/resource) pour cette collection. |
| [isReadOnly()](#isReadOnly--) | Obtient une valeur indiquant si cette collection est en lecture seule. |
| [iterator()](#iterator--) | Renvoie un énumérateur pour cette collection. |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | Supprime l'instance Rate de cette collection. |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | Définit l'élément à l'index spécifié. |
| [size()](#size--) | Obtient le nombre d'éléments contenus dans le RateCollection. |
| [toList()](#toList--) | Convertit l'objet [RateCollection](../../com.aspose.tasks/ratecollection) en une liste d'objets [Rate](../../com.aspose.tasks/rate). |
| [toList(int type)](#toList-int-) | Convertit l'objet [RateCollection](../../com.aspose.tasks/ratecollection) en une liste d'objets [Rate](../../com.aspose.tasks/rate) filtrés par le type [RateType](../../com.aspose.tasks/ratetype) spécifié. |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


Ajoute une nouvelle instance [Rate](../../com.aspose.tasks/rate) à cette collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ratesFrom | java.util.Date | La date à laquelle le nouveau taux entre en vigueur. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


Ajoute une nouvelle instance [Rate](../../com.aspose.tasks/rate) à cette collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ratesFrom | java.util.Date | La date à laquelle le nouveau taux entre en vigueur. |
| type | int | Le tableau de taux dans lequel ajouter. |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


Renvoie l'élément à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| key | int | L'index basé sur zéro de l'élément à obtenir. |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


Obtient l'objet parent [Resource](../../com.aspose.tasks/resource) pour cette collection.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Obtient une valeur indiquant si cette collection est en lecture seule.

**Returns:**
boolean - une valeur indiquant si cette collection est en lecture seule.
### iterator() {#iterator--}
```
public final Iterator iterator()
```


Renvoie un énumérateur pour cette collection.

**Returns:**
java.util.Iterator - un énumérateur pour cette collection.
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| key | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


Supprime l'instance Rate de cette collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | L'élément à supprimer. |

**Returns:**
boolean - true si le Rate spécifié a été supprimé avec succès ; sinon, false.
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


Définit l'élément à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| key | int | L'index basé sur zéro de l'élément à définir. |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | L'élément à définir à l'index spécifié. |

### size() {#size--}
```
public final int size()
```


Obtient le nombre d'éléments contenus dans le RateCollection.

**Returns:**
int - le nombre d'éléments contenus dans le RateCollection.
### toList() {#toList--}
```
public final List<Rate> toList()
```


Convertit l'objet [RateCollection](../../com.aspose.tasks/ratecollection) en une liste d'objets [Rate](../../com.aspose.tasks/rate).

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - Liste d'objets [Rate](../../com.aspose.tasks/rate).
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


Convertit l'objet [RateCollection](../../com.aspose.tasks/ratecollection) en une liste d'objets [Rate](../../com.aspose.tasks/rate) filtrés par le type [RateType](../../com.aspose.tasks/ratetype) spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | Le type sur lequel filtrer. |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - une liste d'objets [Rate](../../com.aspose.tasks/rate).
