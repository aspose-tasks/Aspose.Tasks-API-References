---
title: "ViewCollection"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Περιέχει μια λίστα από αντικείμενα."
type: docs
weight: 343
url: /el/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

Περιέχει μια λίστα από αντικείμενα [View](../../com.aspose.tasks/view). Επεκτείνει την κλάση `AbstractCollection`.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή. |
| [clear()](#clear--) | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή. |
| [contains(View item)](#contains-com.aspose.tasks.View-) | Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false. |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τον καθορισμένο δείκτη πίνακα. |
| [getByName(String viewName)](#getByName-java.lang.String-) | Αναζητά ένα View με το όνομα και επιστρέφει την πρώτη εμφάνιση μέσα στη συλλογή. |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | Αναζητά ένα View με την καθορισμένη ιδιότητα Screen και επιστρέφει την πρώτη εμφάνιση μέσα στη συλλογή. |
| [getParentProject()](#getParentProject--) | Λαμβάνει το γονικό αντικείμενο του View. |
| [iterator()](#iterator--) | Επιστρέφει έναν iterator για τα στοιχεία που περιέχονται σε αυτή τη συλλογή. |
| [remove(View item)](#remove-com.aspose.tasks.View-) | Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή. |
| [size()](#size--) | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή. |
| [toList()](#toList--) | Μετατρέπει μια συλλογή προβολών σε λίστα από αντικείμενα [View](../../com.aspose.tasks/view). |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | το καθορισμένο στοιχείο για προσθήκη σε αυτή τη συλλογή. |

**Returns:**
boolean - true εάν η λειτουργία ήταν επιτυχής.
### clear() {#clear--}
```
public final void clear()
```


Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή.

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | το καθορισμένο στοιχείο για εύρεση. |

**Returns:**
boolean - true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false.
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τον καθορισμένο δείκτη πίνακα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | ο καθορισμένος μονοδιάστατος πίνακας στον οποίο θα αντιγραφούν τα στοιχεία |
| arrayIndex | int | ο δείκτης μηδενικής βάσης του καθορισμένου πίνακα στο οποίο αρχίζει η αντιγραφή. |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


Αναζητά ένα View με το όνομα και επιστρέφει την πρώτη εμφάνιση μέσα στη συλλογή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| viewName | java.lang.String | Όνομα του View για αναζήτηση. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


Αναζητά ένα View με την καθορισμένη ιδιότητα Screen και επιστρέφει την πρώτη εμφάνιση μέσα στη συλλογή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| screen | int | Τιμή απαρίθμησης [ViewScreen](../../com.aspose.tasks/viewscreen). |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Λαμβάνει το γονικό αντικείμενο του View. Μόνο για ανάγνωση [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


Επιστρέφει έναν iterator για τα στοιχεία που περιέχονται σε αυτή τη συλλογή.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - iterator συλλογής.
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | το καθορισμένο αντικείμενο για αφαίρεση. |

**Returns:**
boolean - true εάν το καθορισμένο αντικείμενο αφαιρέθηκε επιτυχώς από αυτή τη συλλογή· διαφορετικά, false.
### size() {#size--}
```
public final int size()
```


Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή.

**Returns:**
int - ο αριθμός των στοιχείων που περιέχονται σε αυτή τη συλλογή.
### toList() {#toList--}
```
public final List<View> toList()
```


Μετατρέπει μια συλλογή προβολών σε λίστα από αντικείμενα [View](../../com.aspose.tasks/view).

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - Γενική λίστα αντικειμένων [View](../../com.aspose.tasks/view).
