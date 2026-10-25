---
title: "PropertyKeyedCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Una classe base di una raccolta di proprietà."
type: docs
weight: 231
url: /it/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

Una classe base di una raccolta di proprietà.

T : il tipo di proprietà.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \{@inheritDoc\} |
| [add(T item)](#add-T-) | Crea una nuova proprietà personalizzata. |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object item)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [contains(String name)](#contains-java.lang.String-) | Determina se la Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; contiene una proprietà con il nome specificato. |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \{@inheritDoc\} |
| [getNames()](#getNames--) | Restituisce la raccolta di tutti i nomi delle proprietà. |
| [get_Item(String name)](#get-Item-java.lang.String-) | Restituisce la Property associata alla chiave specificata. |
| [isEmpty()](#isEmpty--) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Ottiene un valore che indica se questa collezione è di sola lettura; altrimenti, false. |
| [remove(Object item)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \{@inheritDoc\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \{@inheritDoc\} |
| [size()](#size--) | Restituisce il numero di proprietà nella raccolta. |
| [toArray()](#toArray--) | \{@inheritDoc\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | T1[] | \{@inheritDoc\} |

**Returns:**
T1[] - \{@inheritDoc\}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Crea una nuova proprietà personalizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | T | La proprietà da aggiungere. |

**Returns:**
boolean
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| c | java.util.Collection&lt;? extends T&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public void clear()
```




### contains(Object item) {#contains-java.lang.Object-}
```
public final boolean contains(Object item)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | java.lang.Object |  |

**Returns:**
boolean
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


Determina se la Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; contiene una proprietà con il nome specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome di una proprietà |

**Returns:**
boolean - true se la Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; contiene una proprietà con il nome specificato; altrimenti, false.
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


Restituisce la raccolta di tutti i nomi delle proprietà.

**Returns:**
java.util.Collection&lt;java.lang.String&gt; - la raccolta di tutti i nomi delle proprietà.
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


Restituisce la Property associata alla chiave specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della Property da ottenere. |

**Returns:**
T - La Property associata al nome specificato.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```




**Returns:**
boolean - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Ottiene un valore che indica se questa collezione è di sola lettura; altrimenti, false.

**Returns:**
boolean - un valore che indica se questa collezione è di sola lettura; altrimenti, false.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Restituisce il numero di proprietà nella raccolta.

**Returns:**
int - il numero di proprietà nella raccolta.
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - \{@inheritDoc\}
