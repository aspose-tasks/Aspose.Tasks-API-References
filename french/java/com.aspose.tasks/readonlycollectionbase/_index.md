---
title: "ReadOnlyCollectionBase"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une collection en lecture seule d'objets."
type: docs
weight: 238
url: /fr/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

Représente une collection en lecture seule d'objets.

T : type des éléments de la collection.
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(T item)](#add-T-) | Ceci est l’implémentation factice de la méthode Add de ICollection, qui ne fait que lever UnsupportedOperationException. |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | Renvoie l'élément à l'index spécifié. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Détermine si la collection est en lecture seule. |
| [iterator()](#iterator--) | Renvoie un énumérateur pour cette collection. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | Renvoie l'élément à l'index spécifié. |
| [size()](#size--) | Obtient le nombre d’objets contenus dans l’objet. |
| [toList()](#toList--) | Convertit la collection en une liste d’objets. |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Ceci est l’implémentation factice de la méthode Add de ICollection, qui ne fait que lever UnsupportedOperationException.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| élément | T | L’élément à ajouter. |

**Returns:**
booléen
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | \{@inheritDoc\} |
| élément | T | \{@inheritDoc\} |

### clear() {#clear--}
```
public final void clear()
```




### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


Renvoie l'élément à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | L'index basé sur zéro de l'élément à obtenir. |

**Returns:**
T - l’élément à l’indice spécifié.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Détermine si la collection est en lecture seule.

**Returns:**
boolean - vrai si la collection est en lecture seule ; faux sinon.
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


Renvoie un énumérateur pour cette collection.

**Returns:**
java.util.Iterator<T> - un itérateur pour cette collection.
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | \{@inheritDoc\} |

**Returns:**
T - {@inheritDoc}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


Renvoie l'élément à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | L'index basé sur zéro de l'élément à obtenir. |
| valeur | T |  |

**Returns:**
T - l’élément à l’indice spécifié.
### size() {#size--}
```
public final int size()
```


Obtient le nombre d’objets contenus dans l’objet.

**Returns:**
int - le nombre d’objets contenus dans l’objet.
### toList() {#toList--}
```
public final List<T> toList()
```


Convertit la collection en une liste d’objets.

**Returns:**
java.util.List<T> - liste générique d’objets.
