---
title: "CustomProjectPropertyCollection"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια συλλογή προσαρμοσμένων ιδιοτήτων έργου."
type: docs
weight: 61
url: /el/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

Αντιπροσωπεύει μια συλλογή προσαρμοσμένων ιδιοτήτων έργου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα. |
| [add(String name, double value)](#add-java.lang.String-double-) | Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα. |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα. |
| [clear()](#clear--) | Καθαρίζει το PropertyCollection. |
| [isReadOnly()](#isReadOnly--) | Λαμβάνει μια τιμή που υποδεικνύει αν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, ψευδής. |
| [remove(String name)](#remove-java.lang.String-) | Αφαιρεί μια ιδιότητα με το καθορισμένο όνομα από τη συλλογή. |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection).

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Το όνομα της ιδιότητας. |
| τιμή | boolean | Η τιμή του νεοδημιουργημένου αντικειμένου ιδιότητας. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Το όνομα της ιδιότητας. |
| τιμή | double | Η τιμή του νεοδημιουργημένου αντικειμένου ιδιότητας. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Το όνομα της ιδιότητας. |
| τιμή | java.lang.String | Η τιμή του νεοδημιουργημένου αντικειμένου ιδιότητας. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Το όνομα της ιδιότητας. |
| τιμή | java.util.Date | Η τιμή του νεοδημιουργημένου αντικειμένου ιδιότητας. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


Καθαρίζει το PropertyCollection.

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Λαμβάνει μια τιμή που υποδεικνύει αν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, ψευδής.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, false.
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


Αφαιρεί μια ιδιότητα με το καθορισμένο όνομα από τη συλλογή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Το όνομα της ιδιότητας χωρίς διάκριση πεζών-κεφαλαίων. |

**Returns:**
boolean - True εάν το στοιχείο βρεθεί και αφαιρεθεί επιτυχώς; διαφορετικά, false.
