---
title: "FieldHelper"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Βοηθητική κλάση που παρέχει χρήσιμες λειτουργίες με πεδία."
type: docs
weight: 88
url: /el/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

Βοηθητική κλάση που παρέχει χρήσιμες λειτουργίες με πεδία.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | Επιστρέφει έναν προεπιλεγμένο τίτλο του συγκεκριμένου πεδίου. |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | Επιστρέφει έναν προεπιλεγμένο τίτλο του συγκεκριμένου πεδίου εργασίας. |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


Επιστρέφει έναν προεπιλεγμένο τίτλο του συγκεκριμένου πεδίου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| πεδίο | int | Πεδίο για λήψη προεπιλεγμένου τίτλου. |

**Returns:**
java.lang.String - Ένας προεπιλεγμένος τίτλος του συγκεκριμένου πεδίου εάν το πεδίο μπορεί να εμφανιστεί στην προβολή του MS Project, αλλιώς null.
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


Επιστρέφει έναν προεπιλεγμένο τίτλο του συγκεκριμένου πεδίου εργασίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| taskKey | byte | Πεδίο εργασίας για λήψη προεπιλεγμένου τίτλου. |

**Returns:**
java.lang.String - Ένας προεπιλεγμένος τίτλος του συγκεκριμένου πεδίου εργασίας εάν το πεδίο μπορεί να εμφανιστεί στην προβολή του MS Project, αλλιώς null.
