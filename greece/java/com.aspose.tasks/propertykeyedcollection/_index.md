---
title: "PropertyKeyedCollection"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Μια βασική κλάση μιας συλλογής ιδιοτήτων."
type: docs
weight: 231
url: /el/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

Μια βασική κλάση μιας συλλογής ιδιοτήτων.

T : ο τύπος της ιδιότητας.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \\{@inheritDoc\\} |
| [add(T item)](#add-T-) | Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα. |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \\{@inheritDoc\\} |
| [clear()](#clear--) | \\{@inheritDoc\\} |
| [contains(Object item)](#contains-java.lang.Object-) | \\{@inheritDoc\\} |
| [contains(String name)](#contains-java.lang.String-) | Καθορίζει εάν η Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; περιέχει μια ιδιότητα με το καθορισμένο όνομα. |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \\{@inheritDoc\\} |
| [getNames()](#getNames--) | Λαμβάνει τη συλλογή όλων των ονομάτων ιδιοτήτων. |
| [get_Item(String name)](#get-Item-java.lang.String-) | Λαμβάνει την Ιδιότητα που σχετίζεται με το καθορισμένο κλειδί. |
| [isEmpty()](#isEmpty--) | \\{@inheritDoc\\} |
| [isReadOnly()](#isReadOnly--) | Λαμβάνει μια τιμή που υποδεικνύει αν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, ψευδής. |
| [remove(Object item)](#remove-java.lang.Object-) | \\{@inheritDoc\\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \\{@inheritDoc\\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \\{@inheritDoc\\} |
| [size()](#size--) | Λαμβάνει τον αριθμό των ιδιοτήτων στη συλλογή. |
| [toArray()](#toArray--) | \\{@inheritDoc\\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ένα | T1[] | \\{@inheritDoc\\} |

**Returns:**
T1[] - \{@inheritDoc\}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| στοιχείο | T | Η ιδιότητα προς προσθήκη. |

**Returns:**
boolean
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| c | java.util.Collection&lt;? extends T&gt; | \\{@inheritDoc\\} |

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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| στοιχείο | java.lang.Object |  |

**Returns:**
boolean
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


Καθορίζει εάν η Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; περιέχει μια ιδιότητα με το καθορισμένο όνομα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Το όνομα μιας ιδιότητας |

**Returns:**
boolean - true εάν η Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; περιέχει μια ιδιότητα με το καθορισμένο όνομα· διαφορετικά, false.
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \\{@inheritDoc\\} |

**Returns:**
boolean - \{@inheritDoc\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


Λαμβάνει τη συλλογή όλων των ονομάτων ιδιοτήτων.

**Returns:**
java.util.Collection&lt;java.lang.String&gt; - η συλλογή όλων των ονομάτων ιδιοτήτων.
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


Λαμβάνει την Ιδιότητα που σχετίζεται με το καθορισμένο κλειδί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Το όνομα της Ιδιότητας προς λήψη. |

**Returns:**
T - Η Ιδιότητα που σχετίζεται με το καθορισμένο όνομα.
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


Λαμβάνει μια τιμή που υποδεικνύει αν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, ψευδής.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, false.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| στοιχείο | java.lang.Object | \\{@inheritDoc\\} |

**Returns:**
boolean - \{@inheritDoc\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \\{@inheritDoc\\} |

**Returns:**
boolean - \{@inheritDoc\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \\{@inheritDoc\\} |

**Returns:**
boolean - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Λαμβάνει τον αριθμό των ιδιοτήτων στη συλλογή.

**Returns:**
int - ο αριθμός των ιδιοτήτων στη συλλογή.
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - \{@inheritDoc\}
