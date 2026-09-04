---
title: "TaskLinkCollection"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια συλλογή από αντικείμενα."
type: docs
weight: 296
url: /el/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

Αναπαριστά μια συλλογή από αντικείμενα [Task](../../com.aspose.tasks/task).
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | Επιστρέφει ένα παράδειγμα του Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) που έχει προστεθεί στο αντικείμενο TaskLinkCollection. |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | Επιστρέφει ένα παράδειγμα του [TaskLink](../../com.aspose.tasks/tasklink) που έχει προστεθεί στο αντικείμενο TaskLinkCollection. |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | Επιστρέφει ένα παράδειγμα του [TaskLink](../../com.aspose.tasks/tasklink) που έχει προστεθεί στο αντικείμενο TaskLinkCollection. |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | Αυτή είναι η ψευδο-εφαρμογή της μεθόδου Add του ICollection, η οποία μόνο ρίχνει UnsupportedOperationException |
| [clear()](#clear--) | Δεσμευμένο για εσωτερική χρήση. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | Αποκτά το γονικό έργο του αντικειμένου ResourceAssignmentCollection. |
| [remove(int index)](#remove-int-) | Αφαιρεί το στοιχείο στη καθορισμένη θέση σε αυτή τη συλλογή και επιστρέφει το στοιχείο που αφαιρέθηκε από τη συλλογή. |
| [remove(Object item)](#remove-java.lang.Object-) | Αφαιρεί σύνδεσμο εργασίας από ένα έργο. |
| [size()](#size--) | Επιστρέφει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο `TaskLinkCollection`. |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \\{@inheritDoc\\} |
| [toList()](#toList--) | Μετατρέπει το αντικείμενο TaskLinkCollection σε λίστα από αντικείμενα [TaskLink](../../com.aspose.tasks/tasklink). |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


Επιστρέφει ένα παράδειγμα του Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) που έχει προστεθεί στο αντικείμενο TaskLinkCollection.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Προηγούμενη εργασία. |
| succ | [Task](../../com.aspose.tasks/task) | Επόμενη εργασία. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


Επιστρέφει ένα παράδειγμα του [TaskLink](../../com.aspose.tasks/tasklink) που έχει προστεθεί στο αντικείμενο TaskLinkCollection.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Προηγούμενη εργασία. |
| succ | [Task](../../com.aspose.tasks/task) | Επόμενη εργασία. |
| linkType | int | Τύπος συνδέσμου [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


Επιστρέφει ένα παράδειγμα του [TaskLink](../../com.aspose.tasks/tasklink) που έχει προστεθεί στο αντικείμενο TaskLinkCollection.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Προηγούμενη εργασία. |
| succ | [Task](../../com.aspose.tasks/task) | Επόμενη εργασία. |
| linkType | int | Τύπος συνδέσμου [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | Καθυστέρηση συνδέσμου [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


Αυτή είναι η ψευδο-εφαρμογή της μεθόδου Add του ICollection, η οποία μόνο ρίχνει UnsupportedOperationException

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | Το στοιχείο προς προσθήκη. |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Δεσμευμένο για εσωτερική χρήση.

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | \\{@inheritDoc\\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Αποκτά το γονικό έργο του αντικειμένου ResourceAssignmentCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


Αφαιρεί το στοιχείο στη καθορισμένη θέση σε αυτή τη συλλογή και επιστρέφει το στοιχείο που αφαιρέθηκε από τη συλλογή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | η καθορισμένη θέση για αφαίρεση του στοιχείου. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Αφαιρεί σύνδεσμο εργασίας από ένα έργο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| στοιχείο | java.lang.Object | την καθορισμένη παρουσία της κλάσης `TaskLink` προς αφαίρεση. |

**Returns:**
boolean - επιστρέφει την παρουσία της κλάσης `TaskLink` που αφαιρέθηκε από αυτή τη συλλογή.
### size() {#size--}
```
public final int size()
```


Επιστρέφει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο `TaskLinkCollection`. Μόνο για ανάγνωση `int`.

**Returns:**
int - επιστρέφει τον αριθμό των αντικειμένων που περιέχονται σε αυτή τη συλλογή.
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \\{@inheritDoc\\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


Μετατρέπει το αντικείμενο TaskLinkCollection σε λίστα από αντικείμενα [TaskLink](../../com.aspose.tasks/tasklink).

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - Λίστα από αντικείμενα [TaskLink](../../com.aspose.tasks/tasklink).
