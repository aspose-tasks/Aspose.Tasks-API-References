---
title: "FilterCollection"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Περιέχει μια λίστα από αντικείμενα."
type: docs
weight: 92
url: /el/java/com.aspose.tasks/filtercollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class FilterCollection extends AbstractCollection<Filter>
```

Περιέχει μια λίστα από αντικείμενα [Filter](../../com.aspose.tasks/filter). Υλοποιεί τη διεπαφή ICollection&lt;Filter&gt;.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add(Filter item)](#add-com.aspose.tasks.Filter-) |  |
| [clear()](#clear--) | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή (προαιρετική λειτουργία). |
| [contains(Filter item)](#contains-com.aspose.tasks.Filter-) | Επιστρέφει true εάν αυτή η συλλογή περιέχει το καθορισμένο στοιχείο. |
| [copyTo(Filter[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Filter---int-) | Αντιγράφει τα στοιχεία από τον καθορισμένο πίνακα σε αυτή τη συλλογή ξεκινώντας από το καθορισμένο δείκτη. |
| [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη πάνω από τα στοιχεία που περιέχονται σε αυτή τη συλλογή. |
| [remove(Filter item)](#remove-com.aspose.tasks.Filter-) | Αφαιρεί το καθορισμένο στοιχείο από αυτή τη συλλογή. |
| [size()](#size--) | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή. |
| [toList()](#toList--) | Μετατρέπει μια συλλογή φίλτρων σε λίστα αντικειμένων `Filter`. |
### add(Filter item) {#add-com.aspose.tasks.Filter-}
```
public boolean add(Filter item)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) |  |

**Returns:**
boolean
### clear() {#clear--}
```
public void clear()
```


Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή (προαιρετική λειτουργία).

### contains(Filter item) {#contains-com.aspose.tasks.Filter-}
```
public final boolean contains(Filter item)
```


Επιστρέφει true εάν αυτή η συλλογή περιέχει το καθορισμένο στοιχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | το καθορισμένο στοιχείο. |

**Returns:**
boolean - true εάν η συλλογή περιέχει το καθορισμένο στοιχείο.
### copyTo(Filter[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Filter---int-}
```
public final void copyTo(Filter[] array, int arrayIndex)
```


Αντιγράφει τα στοιχεία από τον καθορισμένο πίνακα σε αυτή τη συλλογή ξεκινώντας από το καθορισμένο δείκτη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| array | [Filter\[\]](../../com.aspose.tasks/filter) | ο καθορισμένος μονοδιάστατος πίνακας στον οποίο θα αντιγραφούν τα στοιχεία |
| arrayIndex | int | ο δείκτης μηδενικής βάσης του καθορισμένου πίνακα στο οποίο αρχίζει η αντιγραφή. |

### iterator() {#iterator--}
```
public Iterator<Filter> iterator()
```


Επιστρέφει έναν επαναλήπτη πάνω από τα στοιχεία που περιέχονται σε αυτή τη συλλογή.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Filter&gt; - επαναλήπτης συλλογής.
### remove(Filter item) {#remove-com.aspose.tasks.Filter-}
```
public final boolean remove(Filter item)
```


Αφαιρεί το καθορισμένο στοιχείο από αυτή τη συλλογή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | το καθορισμένο στοιχείο. |

**Returns:**
boolean - true εάν η λειτουργία ήταν επιτυχής.
### size() {#size--}
```
public final int size()
```


Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή.

**Returns:**
int - ο αριθμός των στοιχείων που περιέχονται σε αυτή τη συλλογή.
### toList() {#toList--}
```
public List<Filter> toList()
```


Μετατρέπει μια συλλογή φίλτρων σε λίστα αντικειμένων `Filter`.

**Returns:**
java.util.List&lt;com.aspose.tasks.Filter&gt; - Γενική λίστα αντικειμένων `Filter`.
