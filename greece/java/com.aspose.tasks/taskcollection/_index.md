---
title: "TaskCollection"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια συλλογή από αντικείμενα."
type: docs
weight: 293
url: /el/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

Αναπαριστά μια συλλογή από αντικείμενα [Task](../../com.aspose.tasks/task).
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add()](#add--) | Προσθέτει νέα εργασία στη συλλογή εργασιών του έργου στο ίδιο επίπεδο διάρθρωσης με την τελευταία εργασία. |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | Εισάγει μια νέα εργασία πριν από μια εργασία με το καθορισμένο id και στο ίδιο επίπεδο διάρθρωσης. |
| [add(Task item)](#add-com.aspose.tasks.Task-) | Προσθέτει την καθορισμένη εργασία στο στιγμιότυπο της κλάσης [TaskCollection](../../com.aspose.tasks/taskcollection). |
| [add(String taskName)](#add-java.lang.String-) | Προσθέτει μια νέα εργασία στη συλλογή υποεργασιών. |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | Προσθέτει μια νέα επαναλαμβανόμενη εργασία στη συλλογή υποεργασιών. |
| [clear()](#clear--) | \\{@inheritDoc\\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | Ελέγχει εάν η συλλογή περιέχει το καθορισμένο στοιχείο. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Επιστρέφει μια εργασία με το καθορισμένο Id της οποίας ο πρόγονος είναι η γονική εργασία αυτής της συλλογής. |
| [getByUid(int uid)](#getByUid-int-) | Επιστρέφει μια εργασία με το καθορισμένο Uid της οποίας ο πρόγονος είναι η γονική εργασία αυτής της συλλογής. |
| [getParentProject()](#getParentProject--) | Λαμβάνει το γονικό έργο του αντικειμένου TaskCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \\{@inheritDoc\\} |
| [isReadOnly()](#isReadOnly--) | Αποκτά μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση. |
| [iterator()](#iterator--) | Επιστρέφει έναν enumerator για αυτή τη συλλογή. |
| [remove(Object item)](#remove-java.lang.Object-) | Αυτή είναι η ψευδο-εφαρμογή της μεθόδου Remove του ICollection, η οποία απλώς ρίχνει UnsupportedOperationException |
| [size()](#size--) | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται στη TaskCollection. |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \\{@inheritDoc\\} |
| [toList()](#toList--) | Μετατρέπει το αντικείμενο TaskCollection σε λίστα αντικειμένων [Task](../../com.aspose.tasks/task). |
### add() {#add--}
```
public final Task add()
```


Προσθέτει νέα εργασία στη συλλογή εργασιών του έργου στο ίδιο επίπεδο διάρθρωσης με την τελευταία εργασία.

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


Εισάγει μια νέα εργασία πριν από μια εργασία με το καθορισμένο id και στο ίδιο επίπεδο διάρθρωσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | Οι καθορισμένες παράμετροι για τη δημιουργία επαναλαμβανόμενης εργασίας. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


Προσθέστε την καθορισμένη εργασία στο αντίγραφο της κλάσης [TaskCollection](../../com.aspose.tasks/taskcollection). Εάν το ParentProject.CalculationMode είναι None, ο χρήστης πρέπει να καλέσει το Project.Recalculate() μετά τη χρήση αυτής της μεθόδου (Θα επαναπρογραμματίσει όλες τις εργασίες του έργου (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/τελευταίες ημερομηνίες) και θα υπολογίσει τα εξαρτημένα πεδία όπως τα περιθώρια, η εργασία και τα πεδία κόστους, τα IDs και τα επίπεδα περιγράμματος). Εάν το ParentProject.CalculationMode είναι Manual, η μέθοδος θα υπολογίσει μόνο το ID της εργασίας, το επίπεδο περιγράμματος και τους αριθμούς περιγράμματος αυτόματα. Εάν το ParentProject.CalculationMode είναι Automatic, η μέθοδος επαναπρογραμματίζει αυτόματα όλες τις εργασίες του έργου (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/τελευταίες ημερομηνίες, υπολογίζει τα περιθώρια, την εργασία και τα πεδία κόστους, επανυπολογίζει τα IDs και τα επίπεδα περιγράμματος).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | η καθορισμένη εργασία που πρέπει να προστεθεί σε αυτή τη συλλογή εργασιών. |

**Returns:**
boolean - true εάν η λειτουργία ήταν επιτυχής.
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


Προσθέτει μια νέα εργασία στη συλλογή υποεργασιών.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| taskName | java.lang.String | το καθορισμένο όνομα εργασίας. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


Προσθέτει μια νέα επαναλαμβανόμενη εργασία στη συλλογή υποεργασιών.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| taskName | java.lang.String | το καθορισμένο όνομα εργασίας. |
| beforeTaskId | int | Το καθορισμένο ID μιας εργασίας πριν από την οποία θα εισαχθεί μια νέα εργασία. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns a task which was inserted before a task with the specified id.
### clear() {#clear--}
```
public final void clear()
```




### contains(Task item) {#contains-com.aspose.tasks.Task-}
```
public final boolean contains(Task item)
```


Ελέγχει εάν η συλλογή περιέχει το καθορισμένο στοιχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | Το στοιχείο προς έλεγχο. |

**Returns:**
boolean - true, εάν η συλλογή περιέχει ένα στοιχείο, false διαφορετικά.
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | \\{@inheritDoc\\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


Επιστρέφει μια εργασία με το καθορισμένο Id της οποίας ο πρόγονος είναι η γονική εργασία αυτής της συλλογής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


Επιστρέφει μια εργασία με το καθορισμένο Uid της οποίας ο πρόγονος είναι η γονική εργασία αυτής της συλλογής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Λαμβάνει το γονικό έργο του αντικειμένου TaskCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| o | java.lang.Object | \\{@inheritDoc\\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Αποκτά μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση.
### iterator() {#iterator--}
```
public final Iterator<Task> iterator()
```


Επιστρέφει έναν enumerator για αυτή τη συλλογή.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - ένας απαριθμητής για αυτή τη συλλογή.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Αυτή είναι η ψευδο-εφαρμογή της μεθόδου Remove του ICollection, η οποία απλώς ρίχνει UnsupportedOperationException

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| στοιχείο | java.lang.Object | Το στοιχείο προς αφαίρεση. |

**Returns:**
boolean - `true` εάν το στοιχείο αφαιρέθηκε· `false` διαφορετικά.
### size() {#size--}
```
public final int size()
```


Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται στη TaskCollection.

**Returns:**
int - ο αριθμός των αντικειμένων που περιέχονται στη TaskCollection.
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \\{@inheritDoc\\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


Μετατρέπει το αντικείμενο TaskCollection σε λίστα αντικειμένων [Task](../../com.aspose.tasks/task).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - επιστρέφει μια λίστα που περιέχει τις στιγμές της κλάσης [Task](../../com.aspose.tasks/task) αυτής της συλλογής.
