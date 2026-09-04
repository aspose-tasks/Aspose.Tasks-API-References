---
title: "RateCollection"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια συλλογή που περιέχει αντικείμενα."
type: docs
weight: 234
url: /el/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

Αντιπροσωπεύει μια συλλογή που περιέχει αντικείμενα [Rate](../../com.aspose.tasks/rate).
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | Προσθέτει ένα νέο αντικείμενο [Rate](../../com.aspose.tasks/rate) σε αυτή τη συλλογή. |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | Προσθέτει ένα νέο αντικείμενο [Rate](../../com.aspose.tasks/rate) σε αυτή τη συλλογή. |
| [clear()](#clear--) | \\{@inheritDoc\\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | Επιστρέφει το στοιχείο στον καθορισμένο δείκτη. |
| [getParentResource()](#getParentResource--) | Αποκτά το γονικό αντικείμενο [Resource](../../com.aspose.tasks/resource) για αυτή τη συλλογή. |
| [isReadOnly()](#isReadOnly--) | Αποκτά μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση. |
| [iterator()](#iterator--) | Επιστρέφει έναν enumerator για αυτή τη συλλογή. |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | Αφαιρεί το αντικείμενο Rate από αυτή τη συλλογή. |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | Ορίζει το στοιχείο στον καθορισμένο δείκτη. |
| [size()](#size--) | Αποκτά τον αριθμό των στοιχείων που περιέχονται στη RateCollection. |
| [toList()](#toList--) | Μετατρέπει το αντικείμενο [RateCollection](../../com.aspose.tasks/ratecollection) σε λίστα αντικειμένων [Rate](../../com.aspose.tasks/rate). |
| [toList(int type)](#toList-int-) | Μετατρέπει το αντικείμενο [RateCollection](../../com.aspose.tasks/ratecollection) σε λίστα αντικειμένων [Rate](../../com.aspose.tasks/rate) φιλτραρισμένη κατά τον καθορισμένο τύπο [RateType](../../com.aspose.tasks/ratetype). |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


Προσθέτει ένα νέο αντικείμενο [Rate](../../com.aspose.tasks/rate) σε αυτή τη συλλογή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ratesFrom | java.util.Date | Η ημερομηνία που η νέα τιμή τίθεται σε ισχύ. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


Προσθέτει ένα νέο αντικείμενο [Rate](../../com.aspose.tasks/rate) σε αυτή τη συλλογή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ratesFrom | java.util.Date | Η ημερομηνία που η νέα τιμή τίθεται σε ισχύ. |
| type | int | Ο πίνακας τιμών για προσθήκη. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### clear() {#clear--}
```
public final void clear()
```




### entrySet() {#entrySet--}
```
public Set<Map.Entry<Integer,RateByDateCollection>> entrySet()
```


(@inheritDoc\}

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;java.lang.Integer,com.aspose.tasks.RateByDateCollection&gt;&gt; - \{@inheritDoc\}
### get(Object key) {#get-java.lang.Object-}
```
public final RateByDateCollection get(Object key)
```


(@inheritDoc\}

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| key | java.lang.Object | \\{@inheritDoc\\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


Επιστρέφει το στοιχείο στον καθορισμένο δείκτη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| key | int | Ο μηδενικός δείκτης του στοιχείου για λήψη. |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


Αποκτά το γονικό αντικείμενο [Resource](../../com.aspose.tasks/resource) για αυτή τη συλλογή.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Αποκτά μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση.
### iterator() {#iterator--}
```
public final Iterator iterator()
```


Επιστρέφει έναν enumerator για αυτή τη συλλογή.

**Returns:**
java.util.Iterator - ένας απαριθμητής για αυτή τη συλλογή.
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| key | java.lang.Integer | \\{@inheritDoc\\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \\{@inheritDoc\\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


Αφαιρεί το αντικείμενο Rate από αυτή τη συλλογή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | Το στοιχείο προς αφαίρεση. |

**Returns:**
boolean - true εάν το καθορισμένο Rate αφαιρέθηκε επιτυχώς· διαφορετικά, false.
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


Ορίζει το στοιχείο στον καθορισμένο δείκτη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| key | int | Ο δείκτης που αρχίζει από το μηδέν του στοιχείου που θα οριστεί. |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | Το στοιχείο που θα οριστεί στον καθορισμένο δείκτη. |

### size() {#size--}
```
public final int size()
```


Αποκτά τον αριθμό των στοιχείων που περιέχονται στη RateCollection.

**Returns:**
int - ο αριθμός των στοιχείων που περιέχονται στο RateCollection.
### toList() {#toList--}
```
public final List<Rate> toList()
```


Μετατρέπει το αντικείμενο [RateCollection](../../com.aspose.tasks/ratecollection) σε λίστα αντικειμένων [Rate](../../com.aspose.tasks/rate).

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - Λίστα αντικειμένων [Rate](../../com.aspose.tasks/rate).
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


Μετατρέπει το αντικείμενο [RateCollection](../../com.aspose.tasks/ratecollection) σε λίστα αντικειμένων [Rate](../../com.aspose.tasks/rate) φιλτραρισμένη κατά τον καθορισμένο τύπο [RateType](../../com.aspose.tasks/ratetype).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| type | int | Ο τύπος για φιλτράρισμα. |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - μια λίστα αντικειμένων [Rate](../../com.aspose.tasks/rate).
