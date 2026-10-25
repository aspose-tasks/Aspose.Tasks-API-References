---
title: "TimephasedDataCollection"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια συλλογή από αντικείμενα."
type: docs
weight: 321
url: /el/java/com.aspose.tasks/timephaseddatacollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class TimephasedDataCollection extends AbstractList<TimephasedData>
```

Αντιπροσωπεύει μια συλλογή από αντικείμενα [TimephasedData](../../com.aspose.tasks/timephaseddata).
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [TimephasedDataCollection()](#TimephasedDataCollection--) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add(TimephasedData item)](#add-com.aspose.tasks.TimephasedData-) | Προσθέτει ένα στιγμιότυπο [TimephasedData](../../com.aspose.tasks/timephaseddata) σε αυτό το αντικείμενο συλλογής. |
| [addRange(Iterable&lt;TimephasedData&gt; timephasedCollection)](#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--) | Προσθέτει μια συλλογή από στιγμιότυπα [TimephasedData](../../com.aspose.tasks/timephaseddata) σε αυτό το αντικείμενο συλλογής. |
| [clear()](#clear--) | Αφαιρεί όλα τα στοιχεία από το [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
| [containsItem(TimephasedData item)](#containsItem-com.aspose.tasks.TimephasedData-) | Καθορίζει εάν το [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) περιέχει μια συγκεκριμένη τιμή. |
| [copyToTArray(TimephasedData[] array, int arrayIndex)](#copyToTArray-com.aspose.tasks.TimephasedData---int-) | Αντιγράφει τα στοιχεία του [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) σε έναν Πίνακα, ξεκινώντας από ένα συγκεκριμένο δείκτη Πίνακα. |
| [get(int index)](#get-int-) | \\{@inheritDoc\\} |
| [isReadOnly()](#isReadOnly--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το System.Collections.Generic.ICollection<T> είναι μόνο για ανάγνωση. |
| [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη για αυτή τη συλλογή. |
| [remove(TimephasedData item)](#remove-com.aspose.tasks.TimephasedData-) | Αφαιρεί το στιγμιότυπο [TimephasedData](../../com.aspose.tasks/timephaseddata) από αυτό το αντικείμενο συλλογής. |
| [selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)](#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-) | Επιλέγει όλες τις χρονικές φάσεις μεταξύ `startTime` και `finishTime`. |
| [set_Item(int index, TimephasedData value)](#set-Item-int-com.aspose.tasks.TimephasedData-) | Ορίζει το στοιχείο στον καθορισμένο δείκτη. |
| [size()](#size--) | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
| [toList()](#toList--) | Μετατρέπει το αντικείμενο [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) σε λίστα αντικειμένων [TimephasedData](../../com.aspose.tasks/timephaseddata). |
### TimephasedDataCollection() {#TimephasedDataCollection--}
```
public TimephasedDataCollection()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

### add(TimephasedData item) {#add-com.aspose.tasks.TimephasedData-}
```
public final boolean add(TimephasedData item)
```


Προσθέτει ένα στιγμιότυπο [TimephasedData](../../com.aspose.tasks/timephaseddata) σε αυτό το αντικείμενο συλλογής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | Το στοιχείο προς προσθήκη. |

**Returns:**
boolean - true, εάν το στοιχείο προστέθηκε· διαφορετικά false.
### addRange(Iterable&lt;TimephasedData&gt; timephasedCollection) {#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--}
```
public final void addRange(Iterable<TimephasedData> timephasedCollection)
```


Προσθέτει μια συλλογή από στιγμιότυπα [TimephasedData](../../com.aspose.tasks/timephaseddata) σε αυτό το αντικείμενο συλλογής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| timephasedCollection | java.lang.Iterable&lt;com.aspose.tasks.TimephasedData&gt; | Μια συλλογή από αντικείμενα [TimephasedData](../../com.aspose.tasks/timephaseddata) προς προσθήκη. |

### clear() {#clear--}
```
public final void clear()
```


Αφαιρεί όλα τα στοιχεία από το [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

### containsItem(TimephasedData item) {#containsItem-com.aspose.tasks.TimephasedData-}
```
public final boolean containsItem(TimephasedData item)
```


Καθορίζει εάν το [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) περιέχει μια συγκεκριμένη τιμή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | Το αντικείμενο προς εντοπισμό στη συλλογή. |

**Returns:**
boolean - true εάν το `item` βρεθεί στη συλλογή· διαφορετικά false.
### copyToTArray(TimephasedData[] array, int arrayIndex) {#copyToTArray-com.aspose.tasks.TimephasedData---int-}
```
public final void copyToTArray(TimephasedData[] array, int arrayIndex)
```


Αντιγράφει τα στοιχεία του [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) σε έναν Πίνακα, ξεκινώντας από ένα συγκεκριμένο δείκτη Πίνακα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| array | [TimephasedData\[\]](../../com.aspose.tasks/timephaseddata) | Ο μονοδιάστατος Πίνακας που είναι ο προορισμός των στοιχείων που αντιγράφηκαν από το [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). Ο Πίνακας πρέπει να έχει μηδενική βάση ευρετηρίου. |
| arrayIndex | int | Ο δείκτης μηδενικής βάσης στο `array` όπου ξεκινά η αντιγραφή. |

### get(int index) {#get-int-}
```
public TimephasedData get(int index)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | \\{@inheritDoc\\} |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το System.Collections.Generic.ICollection<T> είναι μόνο για ανάγνωση.

**Returns:**
boolean - true εάν το System.Collections.Generic.ICollection<T> είναι μόνο για ανάγνωση· διαφορετικά, false.
### iterator() {#iterator--}
```
public final Iterator<TimephasedData> iterator()
```


Επιστρέφει έναν επαναλήπτη για αυτή τη συλλογή.

**Returns:**
java.util.Iterator<com.aspose.tasks.TimephasedData> - ένας επαναλήπτης για αυτή τη συλλογή.
### remove(TimephasedData item) {#remove-com.aspose.tasks.TimephasedData-}
```
public final boolean remove(TimephasedData item)
```


Αφαιρεί το στιγμιότυπο [TimephasedData](../../com.aspose.tasks/timephaseddata) από αυτό το αντικείμενο συλλογής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | Το στοιχείο προς αφαίρεση. |

**Returns:**
boolean - true εάν το `item` αφαιρέθηκε επιτυχώς από το [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection); διαφορετικά, false. Αυτή η μέθοδος επιστρέφει επίσης false εάν το `item` δεν βρεθεί στο [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).
### selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime) {#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-}
```
public final List<TimephasedData> selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)
```


Επιλέγει όλες τις φάσεις χρόνου μεταξύ `startTime` και `finishTime`. Έχει πολυπλοκότητα O(log n) στην μέση περίπτωση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| timephasedDataType | byte | Τύπος των φάσεων χρόνου προς επιλογή. |
| startTime | java.util.Date | Η έναρξη του διαστήματος. |
| finishTime | java.util.Date | Το τέλος του διαστήματος. |

**Returns:**
java.util.List<com.aspose.tasks.TimephasedData> - Επιστρέφει νέο αντικείμενο λίστας των δεδομένων του [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) ταξινομημένα κατά την ιδιότητα Start.
### set_Item(int index, TimephasedData value) {#set-Item-int-com.aspose.tasks.TimephasedData-}
```
public final void set_Item(int index, TimephasedData value)
```


Ορίζει το στοιχείο στον καθορισμένο δείκτη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Ο δείκτης που αρχίζει από το μηδέν του στοιχείου που θα οριστεί. |
| value | [TimephasedData](../../com.aspose.tasks/timephaseddata) | το στοιχείο προς ορισμό. |

### size() {#size--}
```
public final int size()
```


Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

**Returns:**
int - ο αριθμός των αντικειμένων που περιέχονται σε αυτό το αντικείμενο [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).
### toList() {#toList--}
```
public final List<TimephasedData> toList()
```


Μετατρέπει το αντικείμενο [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) σε λίστα αντικειμένων [TimephasedData](../../com.aspose.tasks/timephaseddata).

**Returns:**
java.util.List<com.aspose.tasks.TimephasedData> - Λίστα αντικειμένων [TimephasedData](../../com.aspose.tasks/timephaseddata).
