---
title: "TaskLink"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει έναν σύνδεσμο προκάτοχου."
type: docs
weight: 295
url: /el/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

Αντιπροσωπεύει έναν σύνδεσμο προκάτοχου.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [equals(Object obj)](#equals-java.lang.Object-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [getCrossProjectName()](#getCrossProjectName--) | Λαμβάνει το εξωτερικό έργο προκάτοχο. |
| [getLagFormat()](#getLagFormat--) | Λαμβάνει τη μορφή για την έκφραση της μορφής καθυστέρησης. |
| [getLinkLag()](#getLinkLag--) | Λαμβάνει την καθυστέρηση σε δεκάδες του λεπτού ή ποσοστό. |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | Λαμβάνει τη διάρκεια της καθυστέρησης, ανάλογα με το LagFormat. |
| [getLinkType()](#getLinkType--) | Λαμβάνει τον τύπο ενός συνδέσμου. |
| [getPredTask()](#getPredTask--) | Λαμβάνει την εργασία προκάτοχο. |
| [getSuccTask()](#getSuccTask--) | Λαμβάνει την εργασία επακόλουθο. |
| [hashCode()](#hashCode--) | Επιστρέφει μια τιμή κώδικα κατακερματισμού για το παράδειγμα της κλάσης [TaskLink](../../com.aspose.tasks/tasklink). |
| [isCrossProject()](#isCrossProject--) | Λαμβάνει μια τιμή που υποδεικνύει εάν ένας προκάτοχος αποτελεί μέρος άλλου έργου. |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν ένας προκάτοχος αποτελεί μέρος άλλου έργου. |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | Ορίζει το εξωτερικό έργο προκάτοχο. |
| [setLagFormat(byte value)](#setLagFormat-byte-) | Ορίζει τη μορφή για την έκφραση της μορφής καθυστέρησης. |
| [setLinkLag(int value)](#setLinkLag-int-) | Ορίζει την καθυστέρηση σε δεκάδες του λεπτού ή ποσοστό. |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | Ορίζει τη διάρκεια της καθυστέρησης, ανάλογα με το LagFormat. |
| [setLinkType(int value)](#setLinkType-int-) | Ορίζει τον τύπο ενός συνδέσμου. |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | Ορίζει την εργασία προκάτοχο. |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | Ορίζει την εργασία επακόλουθο. |
| [toString()](#toString--) | Επιστρέφει την αναπαράσταση συμβολοσειράς ενός TaskLink. |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | Η καθορισμένη περίπτωση της κλάσης [TaskLink](../../com.aspose.tasks/tasklink) για σύγκριση με αυτήν την περίπτωση. |

**Returns:**
boolean - **True** εάν η καθορισμένη περίπτωση της κλάσης [TaskLink](../../com.aspose.tasks/tasklink) έχει τις ίδιες εργασίες προκάτοχο και επακόλουθο με αυτήν την περίπτωση· διαφορετικά, **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | java.lang.Object | Το αντικείμενο για σύγκριση με αυτήν την παρουσία. |

**Returns:**
boolean - **True** εάν το καθορισμένο αντικείμενο είναι ένα TaskLink που έχει τον ίδιο προκάτοχο και διάδοχο με αυτήν την περίπτωση· διαφορετικά, **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


Λαμβάνει το εξωτερικό έργο προκάτοχο.

**Returns:**
java.lang.String - το εξωτερικό έργο προκάτοχο.
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


Λαμβάνει τη μορφή για την έκφραση της μορφής καθυστέρησης.

**Returns:**
byte - η μορφή για την έκφραση της μορφής καθυστέρησης.
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


Λαμβάνει την καθυστέρηση σε δεκάδες του λεπτού ή ποσοστό.

**Returns:**
int - η καθυστέρηση σε δεκάδες του λεπτού ή ποσοστό.
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


Λαμβάνει τη διάρκεια της καθυστέρησης, ανάλογα με το LagFormat.

**Returns:**
double - διάρκεια καθυστέρησης, ανάλογα με το LagFormat.
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


Λαμβάνει τον τύπο ενός συνδέσμου.

**Returns:**
int - ο τύπος ενός συνδέσμου.
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


Λαμβάνει την εργασία προκάτοχο.

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


Λαμβάνει την εργασία επακόλουθο.

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει μια τιμή κώδικα κατακερματισμού για το παράδειγμα της κλάσης [TaskLink](../../com.aspose.tasks/tasklink).

**Returns:**
int - επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν ένας προκάτοχος αποτελεί μέρος άλλου έργου.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν ένας προκάτοχος αποτελεί μέρος άλλου έργου.
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν ένας προκάτοχος αποτελεί μέρος άλλου έργου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν ένας προκάτοχος αποτελεί μέρος άλλου έργου. |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


Ορίζει το εξωτερικό έργο προκάτοχο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το εξωτερικό έργο προκάτοχο. |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


Ορίζει τη μορφή για την έκφραση της μορφής καθυστέρησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | byte | η μορφή για την έκφραση της μορφής καθυστέρησης. |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


Ορίζει την καθυστέρηση σε δεκάδες του λεπτού ή ποσοστό.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | η καθυστέρηση σε δεκάδες του λεπτού ή ποσοστό. |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


Ορίζει τη διάρκεια της καθυστέρησης, ανάλογα με το LagFormat.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | διάρκεια καθυστέρησης, ανάλογα με το LagFormat. |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


Ορίζει τον τύπο ενός συνδέσμου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο τύπος ενός συνδέσμου. |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


Ορίζει την εργασία προκάτοχο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | η εργασία προκάτοχος. |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


Ορίζει την εργασία επακόλουθο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | η εργασία διάδοχος. |

### toString() {#toString--}
```
public String toString()
```


Επιστρέφει την αναπαράσταση συμβολοσειράς ενός TaskLink. Οι ακριβείς λεπτομέρειες της αναπαράστασης δεν καθορίζονται και ενδέχεται να αλλάξουν.

**Returns:**
java.lang.String - συμβολοσειρά που αντιπροσωπεύει το αντικείμενο TaskLink.
