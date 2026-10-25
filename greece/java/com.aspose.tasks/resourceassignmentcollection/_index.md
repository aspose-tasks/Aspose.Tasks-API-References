---
title: "ResourceAssignmentCollection"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια συλλογή από αντικείμενα."
type: docs
weight: 250
url: /el/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

Αναπαριστά μια συλλογή από αντικείμενα [ResourceAssignment](../../com.aspose.tasks/resourceassignment).
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | Αυτή είναι η ψευδο-εφαρμογή της μεθόδου Add του ICollection, η οποία μόνο ρίχνει UnsupportedOperationException |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | Προσθέτει νέα ανάθεση στη συλλογή ResourceAssignmentCollection. |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | Προσθέτει νέα ανάθεση στη συλλογή ResourceAssignmentCollection. |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | Προσθέτει νέα ανάθεση στη συλλογή ResourceAssignmentCollection. |
| [clear()](#clear--) | Αφαιρεί όλα τα στοιχεία από τη συλλογή. |
| [contains(Object o)](#contains-java.lang.Object-) | \\{@inheritDoc\\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | Επιστρέφει μια ανάθεση με το καθορισμένο uid. |
| [getParentProject()](#getParentProject--) | Αποκτά το γονικό έργο του αντικειμένου ResourceAssignmentCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \\{@inheritDoc\\} |
| [isReadOnly()](#isReadOnly--) | Αποκτά μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση. |
| [iterator()](#iterator--) | Επιστρέφει έναν enumerator για αυτή τη συλλογή. |
| [remove(int index)](#remove-int-) | \\{@inheritDoc\\} |
| [remove(Object o)](#remove-java.lang.Object-) | Αφαιρεί την καθορισμένη ανάθεση από τη συλλογή, εάν δεν είναι μόνο για ανάγνωση, διαφορετικά ρίχνει UnsupportedOperationException. |
| [size()](#size--) | Αποκτά τον αριθμό των αντικειμένων που περιέχονται στη συλλογή ResourceAssignmentCollection. |
| [toList()](#toList--) | Μετατρέπει το αντικείμενο ResourceAssignmentCollection σε λίστα από αντικείμενα [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


Αυτή είναι η ψευδο-εφαρμογή της μεθόδου Add του ICollection, η οποία μόνο ρίχνει UnsupportedOperationException

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Το στοιχείο προς αφαίρεση. |

**Returns:**
boolean - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


Προσθέτει νέα ανάθεση στη συλλογή ResourceAssignmentCollection.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Μία εργασία προς ανάθεση. |
| resource | [Resource](../../com.aspose.tasks/resource) | Ένας πόρος προς ανάθεση. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


Προσθέτει νέα ανάθεση στη συλλογή ResourceAssignmentCollection.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Μία εργασία προς ανάθεση. |
| resource | [Resource](../../com.aspose.tasks/resource) | Ένας πόρος προς ανάθεση. |
| μονάδες | double | Ο αριθμός μονάδων για μια νέα ανάθεση. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


Προσθέτει νέα ανάθεση στη συλλογή ResourceAssignmentCollection.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Μία εργασία προς ανάθεση. |
| resource | [Resource](../../com.aspose.tasks/resource) | Ένας πόρος κόστους προς ανάθεση. |
| κόστος | java.math.BigDecimal | Το κόστος για μια νέα ανάθεση. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


Αφαιρεί όλα τα στοιχεία από τη συλλογή.

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| o | java.lang.Object | \\{@inheritDoc\\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public ResourceAssignment get(int index)
```


(@inheritDoc\}

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | \\{@inheritDoc\\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


Επιστρέφει μια ανάθεση με το καθορισμένο uid.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | uid | int | Το καθορισμένο uid. |

--------------------

Συμπλοκότητα O(1). |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Αποκτά το γονικό έργο του αντικειμένου ResourceAssignmentCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
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
public final Iterator<ResourceAssignment> iterator()
```


Επιστρέφει έναν enumerator για αυτή τη συλλογή.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - ένας απαριθμητής για αυτή τη συλλογή.
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | \\{@inheritDoc\\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Αφαιρεί την καθορισμένη ανάθεση από τη συλλογή, εάν δεν είναι μόνο για ανάγνωση, διαφορετικά ρίχνει UnsupportedOperationException.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| o | java.lang.Object | Η ανάθεση για αφαίρεση. |

**Returns:**
boolean - true, εάν το καθορισμένο στοιχείο αφαιρέθηκε, false διαφορετικά.
### size() {#size--}
```
public final int size()
```


Αποκτά τον αριθμό των αντικειμένων που περιέχονται στη συλλογή ResourceAssignmentCollection.

**Returns:**
int - ο αριθμός των αντικειμένων που περιέχονται στη ResourceAssignmentCollection.
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


Μετατρέπει το αντικείμενο ResourceAssignmentCollection σε λίστα από αντικείμενα [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - Λίστα αντικειμένων [ResourceAssignment](../../com.aspose.tasks/resourceassignment).
