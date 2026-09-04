---
title: "PropertyKeyedCollection"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Une classe de base d'une collection de propriétés."
type: docs
weight: 231
url: /fr/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

Une classe de base d'une collection de propriétés.

T : le type de la propriété.
## Méthodes

| Méthode | Description |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \{@inheritDoc\} |
| [add(T item)](#add-T-) | Crée une nouvelle propriété personnalisée. |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object item)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [contains(String name)](#contains-java.lang.String-) | Détermine si la Aspose.Tasks.Properties.PropertyCollection<T> contient une propriété portant le nom spécifié. |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \{@inheritDoc\} |
| [getNames()](#getNames--) | Obtient la collection de tous les noms de propriétés. |
| [get_Item(String name)](#get-Item-java.lang.String-) | Obtient la Propriété associée à la clé spécifiée. |
| [isEmpty()](#isEmpty--) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false. |
| [remove(Object item)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \{@inheritDoc\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \{@inheritDoc\} |
| [size()](#size--) | Obtient le nombre de propriétés dans la collection. |
| [toArray()](#toArray--) | \{@inheritDoc\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | T1[] | \{@inheritDoc\} |

**Returns:**
T1[] - \{@inheritDoc\}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Crée une nouvelle propriété personnalisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| élément | T | La propriété à ajouter. |

**Returns:**
booléen
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| c | java.util.Collection<? extends T> | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### clear() {#clear--}
```
public void clear()
```




### contains(Object item) {#contains-java.lang.Object-}
```
public final boolean contains(Object item)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| élément | java.lang.Object |  |

**Returns:**
booléen
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


Détermine si la Aspose.Tasks.Properties.PropertyCollection<T> contient une propriété portant le nom spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom d'une propriété |

**Returns:**
boolean - vrai si la Aspose.Tasks.Properties.PropertyCollection<T> contient une propriété portant le nom spécifié ; sinon, faux.
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


Obtient la collection de tous les noms de propriétés.

**Returns:**
java.util.Collection<java.lang.String> - la collection de tous les noms de propriétés.
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


Obtient la Propriété associée à la clé spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la Propriété à obtenir. |

**Returns:**
T - La Propriété associée au nom spécifié.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```




**Returns:**
booléen - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false.

**Returns:**
boolean - une valeur indiquant si cette collection est en lecture seule ; sinon, false.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| élément | java.lang.Object | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Obtient le nombre de propriétés dans la collection.

**Returns:**
int - le nombre de propriétés dans la collection.
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - \{@inheritDoc\}
