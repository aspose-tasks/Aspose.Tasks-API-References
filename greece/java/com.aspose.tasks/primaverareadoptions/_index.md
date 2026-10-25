---
title: "PrimaveraReadOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την ανάγνωση αρχείων Primavera Xml ή Primavera Xer."
type: docs
weight: 206
url: /el/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την ανάγνωση αρχείων Primavera Xml ή Primavera Xer.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | Λαμβάνει μια σημαία που καθορίζει εάν τα αρχικά μοναδικά αναγνωριστικά των οντοτήτων πρέπει να διατηρηθούν. |
| [getProjectUid()](#getProjectUid--) | Λαμβάνει το UID ενός έργου για ανάγνωση από αρχείο που περιέχει πολλαπλά έργα. |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | Λαμβάνει μια σημαία που καθορίζει εάν τα έργα βάσης πρέπει να φορτωθούν. |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | Καθορίζει τη συμπεριφορά που χρησιμοποιείται για την επεξεργασία εργασιών με ακαθόριστους περιορισμούς που διαβάζονται από μορφή XER. |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | Ορίζει μια σημαία που καθορίζει εάν τα αρχικά μοναδικά αναγνωριστικά των οντοτήτων πρέπει να διατηρηθούν. |
| [setProjectUid(int value)](#setProjectUid-int-) | Ορίζει το UID ενός έργου για ανάγνωση από αρχείο που περιέχει πολλαπλά έργα. |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | Ορίζει μια σημαία που καθορίζει εάν τα έργα βάσης πρέπει να φορτωθούν. |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | Καθορίζει τη συμπεριφορά που χρησιμοποιείται για την επεξεργασία εργασιών με ακαθόριστους περιορισμούς που διαβάζονται από μορφή XER. |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions).

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


Λαμβάνει μια σημαία που καθορίζει εάν τα αρχικά μοναδικά αναγνωριστικά των οντοτήτων πρέπει να διατηρηθούν.

**Returns:**
boolean - μια σημαία που καθορίζει εάν τα αρχικά μοναδικά αναγνωριστικά των οντοτήτων πρέπει να διατηρηθούν.
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


Λαμβάνει το UID ενός έργου για ανάγνωση από αρχείο που περιέχει πολλαπλά έργα.

**Returns:**
int - το UID ενός έργου για ανάγνωση από αρχείο που περιέχει πολλαπλά έργα.
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


Λαμβάνει μια σημαία που καθορίζει εάν τα έργα βάσης πρέπει να φορτωθούν. Η προεπιλεγμένη τιμή είναι true.

--------------------

Η σημαία εφαρμόζεται σε αρχεία Primavera XML που περιέχουν έργα βάσης (τα baseline δεν υποστηρίζονται από τη μορφή XER). Η επιλογή μπορεί να οριστεί σε false για να επιταχύνει τη φόρτωση ενός μεγάλου έργου με baseline όταν τα δεδομένα baseline δεν χρειάζονται.

**Returns:**
boolean - μια σημαία που καθορίζει εάν τα έργα βάσης πρέπει να φορτωθούν.
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


Καθορίζει τη συμπεριφορά που χρησιμοποιείται για την επεξεργασία εργασιών με ακαθόριστους περιορισμούς που διαβάζονται από μορφή XER.

**Returns:**
int - η συμπεριφορά που χρησιμοποιείται για την επεξεργασία εργασιών με ακαθόριστους περιορισμούς που διαβάζονται από μορφή XER.
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


Ορίζει μια σημαία που καθορίζει εάν τα αρχικά μοναδικά αναγνωριστικά των οντοτήτων πρέπει να διατηρηθούν.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια σημαία που καθορίζει εάν τα αρχικά μοναδικά αναγνωριστικά των οντοτήτων πρέπει να διατηρηθούν. |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


Ορίζει το UID ενός έργου για ανάγνωση από αρχείο που περιέχει πολλαπλά έργα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το UID ενός έργου για ανάγνωση από αρχείο που περιέχει πολλαπλά έργα. |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


Ορίζει μια σημαία που καθορίζει εάν πρέπει να φορτωθούν τα έργα βάσης. Η προεπιλεγμένη τιμή είναι true.

--------------------

Η σημαία εφαρμόζεται σε αρχεία Primavera XML που περιέχουν έργα βάσης (τα baseline δεν υποστηρίζονται από τη μορφή XER). Η επιλογή μπορεί να οριστεί σε false για να επιταχύνει τη φόρτωση ενός μεγάλου έργου με baseline όταν τα δεδομένα baseline δεν χρειάζονται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια σημαία που καθορίζει εάν πρέπει να φορτωθούν τα έργα βάσης. |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


Καθορίζει τη συμπεριφορά που χρησιμοποιείται για την επεξεργασία εργασιών με ακαθόριστους περιορισμούς που διαβάζονται από μορφή XER.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | η συμπεριφορά που χρησιμοποιείται για την επεξεργασία εργασιών με ακαθόριστους περιορισμούς που διαβάζονται από μορφή XER. |

