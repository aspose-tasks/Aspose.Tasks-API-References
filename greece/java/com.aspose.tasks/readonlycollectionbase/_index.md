---
title: "ReadOnlyCollectionBase"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά μια συλλογή αντικειμένων μόνο για ανάγνωση."
type: docs
weight: 238
url: /el/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

Αναπαριστά μια συλλογή αντικειμένων μόνο για ανάγνωση.

T : Τύπος των στοιχείων της συλλογής.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add(T item)](#add-T-) | Αυτή είναι η ψευδο-εφαρμογή της μεθόδου Add του ICollection, η οποία μόνο ρίχνει UnsupportedOperationException |
| [add(int index, T element)](#add-int-T-) | \\{@inheritDoc\\} |
| [clear()](#clear--) | \\{@inheritDoc\\} |
| [contains(Object o)](#contains-java.lang.Object-) | \\{@inheritDoc\\} |
| [get(int index)](#get-int-) | Επιστρέφει το στοιχείο στον καθορισμένο δείκτη. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \\{@inheritDoc\\} |
| [isReadOnly()](#isReadOnly--) | Καθορίζει εάν η συλλογή είναι μόνο για ανάγνωση. |
| [iterator()](#iterator--) | Επιστρέφει έναν enumerator για αυτή τη συλλογή. |
| [remove(int index)](#remove-int-) | \\{@inheritDoc\\} |
| [remove(Object o)](#remove-java.lang.Object-) | \\{@inheritDoc\\} |
| [set(int index, T value)](#set-int-T-) | Επιστρέφει το στοιχείο στον καθορισμένο δείκτη. |
| [size()](#size--) | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται στο αντικείμενο. |
| [toList()](#toList--) | Μετατρέπει τη συλλογή σε λίστα αντικειμένων. |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Αυτή είναι η ψευδο-εφαρμογή της μεθόδου Add του ICollection, η οποία μόνο ρίχνει UnsupportedOperationException

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| στοιχείο | T | Το στοιχείο προς προσθήκη. |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | \\{@inheritDoc\\} |
| στοιχείο | T | \\{@inheritDoc\\} |

### clear() {#clear--}
```
public final void clear()
```




### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| o | java.lang.Object | \\{@inheritDoc\\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


Επιστρέφει το στοιχείο στον καθορισμένο δείκτη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Ο μηδενικός δείκτης του στοιχείου για λήψη. |

**Returns:**
T - το στοιχείο στο καθορισμένο δείκτη.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| o | java.lang.Object | \\{@inheritDoc\\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Καθορίζει εάν η συλλογή είναι μόνο για ανάγνωση.

**Returns:**
boolean - true εάν η συλλογή είναι μόνο για ανάγνωση· false διαφορετικά.
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


Επιστρέφει έναν enumerator για αυτή τη συλλογή.

**Returns:**
java.util.Iterator<T> - Ένας απαριθμητής για αυτή τη συλλογή.
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | \\{@inheritDoc\\} |

**Returns:**
T - {@inheritDoc}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| o | java.lang.Object | \\{@inheritDoc\\} |

**Returns:**
boolean - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


Επιστρέφει το στοιχείο στον καθορισμένο δείκτη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Ο μηδενικός δείκτης του στοιχείου για λήψη. |
| τιμή | T |  |

**Returns:**
T - το στοιχείο στο καθορισμένο δείκτη.
### size() {#size--}
```
public final int size()
```


Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται στο αντικείμενο.

**Returns:**
int - ο αριθμός των αντικειμένων που περιέχονται στο αντικείμενο.
### toList() {#toList--}
```
public final List<T> toList()
```


Μετατρέπει τη συλλογή σε λίστα αντικειμένων.

**Returns:**
java.util.List<T> - Γενική λίστα αντικειμένων.
