---
title: "TaskBaseline"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει το Baseline μιας εργασίας."
type: docs
weight: 291
url: /el/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

Αντιπροσωπεύει το Baseline μιας εργασίας.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | Υλοποίηση διεπαφής IComparable. |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο TaskBaseline. |
| [equals(Object obj)](#equals-java.lang.Object-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [getDuration()](#getDuration--) | Λαμβάνει τη προγραμματισμένη διάρκεια της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |
| [getEstimatedDuration()](#getEstimatedDuration--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η διάρκεια της βάσης αναφοράς της εργασίας ήταν εκτιμώμενη. |
| [getFinish()](#getFinish--) | Λαμβάνει την προγραμματισμένη ημερομηνία λήξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |
| [getFixedCost()](#getFixedCost--) | Λαμβάνει ένα σταθερό κόστος της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |
| [getInterim()](#getInterim--) | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή είναι μια Ενδιάμεση Βάση Αναφοράς. |
| [getStart()](#getStart--) | Λαμβάνει την προγραμματισμένη ημερομηνία έναρξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |
| [getTimephasedData()](#getTimephasedData--) | Λαμβάνει μια παρουσία του TimephasedDataCollection για αυτό το αντικείμενο. |
| [hashCode()](#hashCode--) | Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Ορίζει τη προγραμματισμένη διάρκεια της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν η διάρκεια της βάσης αναφοράς της εργασίας ήταν εκτιμώμενη. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Ορίζει την προγραμματισμένη ημερομηνία λήξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |
| [setFixedCost(double value)](#setFixedCost-double-) | Ορίζει ένα σταθερό κόστος της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |
| [setInterim(boolean value)](#setInterim-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν αυτή είναι ενδιάμεση βάση αναφοράς. |
| [setStart(Date value)](#setStart-java.util.Date-) | Ορίζει την προγραμματισμένη ημερομηνία έναρξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Ορίζει μια παρουσία TimephasedDataCollection για αυτό το αντικείμενο. |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Η γονική εργασία της βάσης αναφοράς. |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


Υλοποίηση διεπαφής IComparable. Συγκρίνει αυτήν την περίπτωση με το καθορισμένο αντικείμενο Baseline.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | το καθορισμένο αντικείμενο Baseline για σύγκριση με αυτήν την περίπτωση. |

**Returns:**
int - επιστρέφει -1 εάν αυτή η περίπτωση είναι μικρότερη από το καθορισμένο αντικείμενο, 1 εάν αυτή η περίπτωση είναι μεγαλύτερη από το καθορισμένο αντικείμενο· διαφορετικά επιστρέφει 0
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο TaskBaseline.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | το καθορισμένο αντικείμενο AssignmentBaseline για σύγκριση με αυτή την παρουσία. |

**Returns:**
boolean - επιστρέφει true εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο TaskBaseline· διαφορετικά, false.
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
boolean - **True** εάν το καθορισμένο αντικείμενο είναι ένα TaskBaseline που έχει την ίδια τιμή UID με αυτή την παρουσία· διαφορετικά, **false**.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Λαμβάνει τη προγραμματισμένη διάρκεια της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η διάρκεια της βάσης αναφοράς της εργασίας ήταν εκτιμώμενη.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν η διάρκεια της βάσης αναφοράς της εργασίας ήταν εκτιμώμενη.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Λαμβάνει την προγραμματισμένη ημερομηνία λήξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς.

**Returns:**
java.util.Date - η προγραμματισμένη ημερομηνία λήξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


Λαμβάνει ένα σταθερό κόστος της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς.

**Returns:**
double - ένα σταθερό κόστος της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς.
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή είναι μια Ενδιάμεση Βάση Αναφοράς.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν αυτή είναι ενδιάμεση βάση αναφοράς.
### getStart() {#getStart--}
```
public final Date getStart()
```


Λαμβάνει την προγραμματισμένη ημερομηνία έναρξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς.

**Returns:**
java.util.Date - η προγραμματισμένη ημερομηνία έναρξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Λαμβάνει μια παρουσία TimephasedDataCollection για αυτό το αντικείμενο. Τα δεδομένα χρονικής φάσης που σχετίζονται με τη βάση αναφοράς της εργασίας.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Returns:**
int - επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Ορίζει τη προγραμματισμένη διάρκεια της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | η προγραμματισμένη διάρκεια της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν η διάρκεια της βάσης αναφοράς της εργασίας ήταν εκτιμώμενη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν η διάρκεια της βάσης αναφοράς της εργασίας ήταν εκτιμώμενη. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Ορίζει την προγραμματισμένη ημερομηνία λήξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η προγραμματισμένη ημερομηνία λήξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


Ορίζει ένα σταθερό κόστος της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | ένα σταθερό κόστος της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν αυτή είναι ενδιάμεση βάση αναφοράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν αυτή είναι ενδιάμεση βάση αναφοράς. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Ορίζει την προγραμματισμένη ημερομηνία έναρξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η προγραμματισμένη ημερομηνία έναρξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Ορίζει μια παρουσία TimephasedDataCollection για αυτό το αντικείμενο. Τα δεδομένα χρονικής φάσης που σχετίζονται με τη βάση αναφοράς της εργασίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | μια παρουσία TimephasedDataCollection για αυτό το αντικείμενο. |

