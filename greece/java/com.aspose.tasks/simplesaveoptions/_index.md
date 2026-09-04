---
title: "SimpleSaveOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αυτή είναι μια αφηρημένη βασική κλάση που επιτρέπει στον χρήστη να καθορίζει βασικές επιλογές κατά την αποθήκευση ενός έργου σε συγκεκριμένη μορφή."
type: docs
weight: 277
url: /el/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

Αυτή είναι μια αφηρημένη βασική κλάση που επιτρέπει στον χρήστη να καθορίζει βασικές επιλογές κατά την αποθήκευση ενός έργου σε συγκεκριμένη μορφή.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | Λαμβάνει τη μορφή στην οποία θα αποθηκευτεί το έγγραφο εάν χρησιμοποιηθεί αυτό το αντικείμενο επιλογών αποθήκευσης. |
| [getTasksComparer()](#getTasksComparer--) | Λαμβάνει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών. |
| [getTasksFilter()](#getTasksFilter--) | Λαμβάνει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που εμφανίζονται στα γραφήματα Gantt, Φύλλου Εργασιών και Χρήσης Εργασιών. |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | Ορίζει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών. |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Ορίζει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που εμφανίζονται στα γραφήματα Gantt, Φύλλου Εργασιών και Χρήσης Εργασιών. |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


Λαμβάνει τη μορφή στην οποία θα αποθηκευτεί το έγγραφο εάν χρησιμοποιηθεί αυτό το αντικείμενο επιλογών αποθήκευσης.

**Returns:**
int - το [SaveFileFormat](../../com.aspose.tasks/savefileformat) στο οποίο θα αποθηκευτεί το έγγραφο.
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


Λαμβάνει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών.

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - ο συγκριτής για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών.
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


Λαμβάνει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που εμφανίζονται στα γραφήματα Gantt, Φύλλου Εργασιών και Χρήσης Εργασιών.

--------------------

Εάν η τιμή δεν καθοριστεί, χρησιμοποιείται το προεπιλεγμένο φίλτρο που αφαιρεί τις μη ορατές εργασίες -- δηλαδή τις υποεργασίες των συμπτυγμένων εργασιών.

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


Ορίζει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | ο συγκριτής για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών. |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


Ορίζει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που εμφανίζονται στα γραφήματα Gantt, Φύλλου Εργασιών και Χρήσης Εργασιών.

--------------------

Εάν η τιμή δεν καθοριστεί, χρησιμοποιείται το προεπιλεγμένο φίλτρο που αφαιρεί τις μη ορατές εργασίες -- δηλαδή τις υποεργασίες των συμπτυγμένων εργασιών.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | η κατάσταση που χρησιμοποιείται για το φιλτράρισμα των εργασιών που εμφανίζονται σε διαγράμματα Gantt, Task Sheet και Task Usage. |

