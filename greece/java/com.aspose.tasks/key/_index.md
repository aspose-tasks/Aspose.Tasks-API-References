---
title: "Key"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά ένα κλειδί ιδιότητας μιας κλάσης του καθορισμένου τύπου."
type: docs
weight: 139
url: /el/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

Αντιπροσωπεύει ένα κλειδί ιδιότητας μιας κλάσης του καθορισμένου τύπου. Μια παρουσία αυτής της κλάσης χρησιμοποιείται κατά την ανάκτηση ή ορισμό ιδιότητας ενός δοχείου.

T : Ο τύπος της τιμής της ιδιότητας.
K : Ο τύπος του κλειδιού της ιδιότητας.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [Clone()](#Clone--) | Επιστρέφει ένα βαθύ αντίγραφο της παρουσίας. |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | Δημιουργεί ένα βαθύ αντίγραφο της παρουσίασης σε άλλη παρουσίαση. |
| [clone()](#clone--) | \\{@inheritDoc\\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | Επιστρέφει μια τιμή που υποδεικνύει αν η καθορισμένη παρουσία `obj1` είναι ίση με την καθορισμένη παρουσία `obj2`. |
| [equals(Object obj)](#equals-java.lang.Object-) | \\{@inheritDoc\\} |
| [getKeyType()](#getKeyType--) | Αποκτά το κλειδί της ιδιότητας. |
| [hashCode()](#hashCode--) | Επιστρέφει έναν κωδικό κατακερματισμού για την παρουσία της κλάσης Key. |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


Επιστρέφει ένα βαθύ αντίγραφο της παρουσίας.

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


Δημιουργεί ένα βαθύ αντίγραφο της παρουσίασης σε άλλη παρουσίαση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | άλλη παρουσία. |

### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### equals(Key obj1, Key obj2) {#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-}
```
public static boolean equals(Key obj1, Key obj2)
```


Επιστρέφει μια τιμή που υποδεικνύει αν η καθορισμένη παρουσία `obj1` είναι ίση με την καθορισμένη παρουσία `obj2`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | το πρώτο αντικείμενο για σύγκριση. |
| obj2 | com.aspose.tasks.Key | το δεύτερο αντικείμενο για σύγκριση. |

**Returns:**
boolean - επιστρέφει true εάν η καθορισμένη παρουσία `obj1` είναι ίση με την καθορισμένη παρουσία `obj2`; διαφορετικά, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | java.lang.Object | \\{@inheritDoc\\} |

**Returns:**
boolean - \{@inheritDoc\}
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


Αποκτά το κλειδί της ιδιότητας.

**Returns:**
K - το κλειδί της ιδιότητας.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει έναν κωδικό κατακερματισμού για την παρουσία της κλάσης Key.

**Returns:**
int - επιστρέφει έναν κωδικό κατακερματισμού για αυτό το αντικείμενο.
