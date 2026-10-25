---
title: "RateCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una collezione che contiene oggetti."
type: docs
weight: 234
url: /it/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

Rappresenta una collezione che contiene oggetti [Rate](../../com.aspose.tasks/rate).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | Aggiunge una nuova istanza di [Rate](../../com.aspose.tasks/rate) a questa collezione. |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | Aggiunge una nuova istanza di [Rate](../../com.aspose.tasks/rate) a questa collezione. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | Restituisce l'elemento all'indice specificato. |
| [getParentResource()](#getParentResource--) | Ottiene l'oggetto [Resource](../../com.aspose.tasks/resource) genitore per questa collezione. |
| [isReadOnly()](#isReadOnly--) | Ottiene un valore che indica se questa collezione è di sola lettura. |
| [iterator()](#iterator--) | Restituisce un enumeratore per questa collezione. |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | Rimuove l'istanza Rate da questa collezione. |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | Imposta l'elemento all'indice specificato. |
| [size()](#size--) | Ottiene il numero di elementi contenuti nella RateCollection. |
| [toList()](#toList--) | Converte l'oggetto [RateCollection](../../com.aspose.tasks/ratecollection) in un elenco di oggetti [Rate](../../com.aspose.tasks/rate). |
| [toList(int type)](#toList-int-) | Converte l'oggetto [RateCollection](../../com.aspose.tasks/ratecollection) in un elenco di oggetti [Rate](../../com.aspose.tasks/rate) filtrati per il tipo [RateType](../../com.aspose.tasks/ratetype) specificato. |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


Aggiunge una nuova istanza di [Rate](../../com.aspose.tasks/rate) a questa collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ratesFrom | java.util.Date | La data in cui il nuovo tasso entra in vigore. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


Aggiunge una nuova istanza di [Rate](../../com.aspose.tasks/rate) a questa collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ratesFrom | java.util.Date | La data in cui il nuovo tasso entra in vigore. |
| type | int | La tabella delle tariffe in cui aggiungere. |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


Restituisce l'elemento all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | int | L'indice basato su zero dell'elemento da ottenere. |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


Ottiene l'oggetto [Resource](../../com.aspose.tasks/resource) genitore per questa collezione.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Ottiene un valore che indica se questa collezione è di sola lettura.

**Returns:**
boolean - un valore che indica se questa collezione è di sola lettura.
### iterator() {#iterator--}
```
public final Iterator iterator()
```


Restituisce un enumeratore per questa collezione.

**Returns:**
java.util.Iterator - un enumeratore per questa collezione.
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


Rimuove l'istanza Rate da questa collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | L'elemento da rimuovere. |

**Returns:**
boolean - true se il Rate specificato è stato rimosso con successo; altrimenti, false.
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


Imposta l'elemento all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | int | L'indice basato su zero dell'elemento da impostare. |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | L'elemento da impostare all'indice specificato. |

### size() {#size--}
```
public final int size()
```


Ottiene il numero di elementi contenuti nella RateCollection.

**Returns:**
int - il numero di elementi contenuti in RateCollection.
### toList() {#toList--}
```
public final List<Rate> toList()
```


Converte l'oggetto [RateCollection](../../com.aspose.tasks/ratecollection) in un elenco di oggetti [Rate](../../com.aspose.tasks/rate).

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - Elenco di oggetti [Rate](../../com.aspose.tasks/rate).
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


Converte l'oggetto [RateCollection](../../com.aspose.tasks/ratecollection) in un elenco di oggetti [Rate](../../com.aspose.tasks/rate) filtrati per il tipo [RateType](../../com.aspose.tasks/ratetype) specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | Il tipo su cui filtrare. |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - un elenco di oggetti [Rate](../../com.aspose.tasks/rate).
