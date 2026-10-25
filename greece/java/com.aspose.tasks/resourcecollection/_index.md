---
title: "ResourceCollection"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια συλλογή από αντικείμενα."
type: docs
weight: 251
url: /el/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

Αναπαριστά μια συλλογή αντικειμένων [Resource](../../com.aspose.tasks/resource).
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add()](#add--) | Προσθέτει νέο πόρο στην τελευταία θέση της συλλογής πόρων ενός έργου. |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \\{@inheritDoc\\} |
| [add(String resourceName)](#add-java.lang.String-) | Προσθέτει νέο πόρο στην τελευταία θέση της συλλογής πόρων ενός έργου. |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | Προσθέτει νέο πόρο στη συγκεκριμένη θέση μιας συλλογής πόρων έργου. |
| [clear()](#clear--) | Η άμεση εκκαθάριση δεν υποστηρίζεται, αυτή η μέθοδος απλώς ρίχνει UnsupportedOperationException. |
| [contains(Object o)](#contains-java.lang.Object-) | \\{@inheritDoc\\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Επιστρέφει έναν πόρο με το συγκεκριμένο αναγνωριστικό. |
| [getByUid(int uid)](#getByUid-int-) | Επιστρέφει έναν πόρο με το συγκεκριμένο Uid. |
| [getParentProject()](#getParentProject--) | Αποκτά το γονικό έργο του αντικειμένου ResourceCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \\{@inheritDoc\\} |
| [isReadOnly()](#isReadOnly--) | \\{@inheritDoc\\} |
| [iterator()](#iterator--) | Επιστρέφει έναν enumerator για αυτή τη συλλογή. |
| [remove(Object o)](#remove-java.lang.Object-) | Αυτή είναι η ψευδο-εφαρμογή της μεθόδου remove της Collection, η οποία μόνο ρίχνει UnsupportedOperationException. |
| [size()](#size--) | Αποκτά τον αριθμό των στοιχείων που περιέχονται στο ResourceCollection. |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \\{@inheritDoc\\} |
| [toList()](#toList--) | Μετατρέπει το αντικείμενο ResourceCollection σε λίστα αντικειμένων [Resource](../../com.aspose.tasks/resource). |
### add() {#add--}
```
public final Resource add()
```


Προσθέτει νέο πόρο στην τελευταία θέση της συλλογής πόρων ενός έργου.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \\{@inheritDoc\\} |

**Returns:**
boolean - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


Προσθέτει νέο πόρο στην τελευταία θέση της συλλογής πόρων ενός έργου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| resourceName | java.lang.String | Όνομα ενός πόρου. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


Προσθέτει νέο πόρο στη συγκεκριμένη θέση μιας συλλογής πόρων έργου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| resourceName | java.lang.String | Όνομα ενός πόρου. |
| beforeResourceId | int | Θέση του προηγούμενου πόρου σε μια συλλογή πόρων έργου. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


Η άμεση εκκαθάριση δεν υποστηρίζεται, αυτή η μέθοδος απλώς ρίχνει UnsupportedOperationException.

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
public Resource get(int index)
```


(@inheritDoc\}

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | \\{@inheritDoc\\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


Επιστρέφει έναν πόρο με το συγκεκριμένο αναγνωριστικό.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | id | int | Το συγκεκριμένο αναγνωριστικό. |

--------------------

Συμπλοκότητα O(1). |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


Επιστρέφει έναν πόρο με το συγκεκριμένο Uid.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | uid | int | Το καθορισμένο uid. |

--------------------

Συμπλοκότητα O(1). |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Αποκτά το γονικό έργο του αντικειμένου ResourceCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
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




**Returns:**
boolean - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


Επιστρέφει έναν enumerator για αυτή τη συλλογή.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - ένας απαριθμητής για αυτή τη συλλογή.
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Αυτή είναι η ψευδο-εφαρμογή της μεθόδου remove της Collection, η οποία μόνο ρίχνει UnsupportedOperationException.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| o | java.lang.Object | το στοιχείο προς αφαίρεση. |

**Returns:**
boolean - `true` εάν το στοιχείο αφαιρέθηκε· `false` διαφορετικά.
### size() {#size--}
```
public final int size()
```


Αποκτά τον αριθμό των στοιχείων που περιέχονται στο ResourceCollection.

--------------------

Μόνο για ανάγνωση `int`.

**Returns:**
int - ο αριθμός των στοιχείων που περιέχονται στο ResourceCollection.
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| comparer | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \\{@inheritDoc\\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


Μετατρέπει το αντικείμενο ResourceCollection σε λίστα αντικειμένων [Resource](../../com.aspose.tasks/resource).

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - Λίστα αντικειμένων [Resource](../../com.aspose.tasks/resource).
