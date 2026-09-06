---
title: "PropertyKeyedCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Una clase base de una colección de propiedades."
type: docs
weight: 231
url: /es/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

Una clase base de una colección de propiedades.

T : el tipo de propiedad.
## Métodos

| Método | Descripción |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \{@inheritDoc\} |
| [add(T item)](#add-T-) | Crea una nueva propiedad personalizada. |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object item)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [contains(String name)](#contains-java.lang.String-) | Determina si la Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; contiene una propiedad con el nombre especificado. |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \{@inheritDoc\} |
| [getNames()](#getNames--) | Obtiene la colección de todos los nombres de propiedades. |
| [get_Item(String name)](#get-Item-java.lang.String-) | Obtiene la Property asociada con la clave especificada. |
| [isEmpty()](#isEmpty--) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Obtiene un valor que indica si esta colección es de solo lectura; de lo contrario, false. |
| [remove(Object item)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \{@inheritDoc\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \{@inheritDoc\} |
| [size()](#size--) | Obtiene el número de propiedades en la colección. |
| [toArray()](#toArray--) | \{@inheritDoc\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | T1[] | \{@inheritDoc\} |

**Returns:**
T1[] - \{@inheritDoc\}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Crea una nueva propiedad personalizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | T | La propiedad a añadir. |

**Returns:**
boolean
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | java.lang.Object |  |

**Returns:**
boolean
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


Determina si la Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; contiene una propiedad con el nombre especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de una propiedad |

**Returns:**
boolean - true si la Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; contiene una propiedad con el nombre especificado; de lo contrario, false.
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


Obtiene la colección de todos los nombres de propiedades.

**Returns:**
java.util.Collection&lt;java.lang.String&gt; - la colección de todos los nombres de propiedades.
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


Obtiene la Property asociada con la clave especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la Property a obtener. |

**Returns:**
T - La Property asociada con el nombre especificado.
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


Obtiene un valor que indica si esta colección es de solo lectura; de lo contrario, false.

**Returns:**
boolean - un valor que indica si esta colección es de solo lectura; de lo contrario, false.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Obtiene el número de propiedades en la colección.

**Returns:**
int - el número de propiedades en la colección.
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - \{@inheritDoc\}
