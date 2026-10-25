---
title: "CalendarCollection"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια συλλογή από αντικείμενα."
type: docs
weight: 42
url: /el/java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

Αντιπροσωπεύει μια συλλογή από αντικείμενα [Calendar](../../com.aspose.tasks/calendar).
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | Προσθέτει ένα νέο βασικό ημερολόγιο σε αυτό το αντικείμενο CalendarCollection και επιστρέφει το προστιθέμενο ημερολόγιο. |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | Προσθέτει ένα νέο ημερολόγιο με το καθορισμένο βασικό ημερολόγιο σε αυτό το αντικείμενο CalendarCollection και επιστρέφει το προστιθέμενο ημερολόγιο. |
| [clear()](#clear--) | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByName(String name)](#getByName-java.lang.String-) | Επιστρέφει ένα ημερολόγιο με το καθορισμένο όνομα. |
| [getByUid(int uid)](#getByUid-int-) | Επιστρέφει ένα ημερολόγιο με το καθορισμένο UID. |
| [iterator()](#iterator--) | Επιστρέφει έναν enumerator για αυτή τη συλλογή. |
| [remove(int index)](#remove-int-) | Αφαιρεί το στοιχείο στη συγκεκριμένη θέση σε αυτή τη λίστα. |
| [remove(Object item)](#remove-java.lang.Object-) | Αφαιρεί το Calendar από το Project CalendarCollection. |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | Αντικαθιστά το στοιχείο στη συγκεκριμένη θέση σε αυτή τη λίστα με το καθορισμένο στοιχείο. |
| [size()](#size--) | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο [CalendarCollection](../../com.aspose.tasks/calendarcollection). |
| [toList()](#toList--) | Μετατρέπει το αντικείμενο CalendarCollection σε λίστα αντικειμένων [Calendar](../../com.aspose.tasks/calendar). |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


Προσθέτει ένα νέο βασικό ημερολόγιο σε αυτό το αντικείμενο CalendarCollection και επιστρέφει το προστιθέμενο ημερολόγιο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Όνομα ημερολογίου. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


Προσθέτει ένα νέο ημερολόγιο με το καθορισμένο βασικό ημερολόγιο σε αυτό το αντικείμενο CalendarCollection και επιστρέφει το προστιθέμενο ημερολόγιο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Καθορισμένο όνομα. |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | Καθορισμένο βασικό ημερολόγιο. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή.

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\}

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | \\{@inheritDoc\\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


Επιστρέφει ένα ημερολόγιο με το καθορισμένο όνομα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Όνομα ενός ημερολογίου. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


Επιστρέφει ένα ημερολόγιο με το καθορισμένο UID.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| uid | int | UID ενός ημερολογίου. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


Επιστρέφει έναν enumerator για αυτή τη συλλογή.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - ένας απαριθμητής για αυτή τη συλλογή.
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


Αφαιρεί το στοιχείο στη συγκεκριμένη θέση σε αυτή τη λίστα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | \\{@inheritDoc\\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Αφαιρεί το Calendar από το Project CalendarCollection.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| στοιχείο | java.lang.Object | Το ημερολόγιο προς αφαίρεση. |

**Returns:**
boolean - Εάν αφαιρεθεί, επιστρέφει true, αλλιώς επιστρέφει false.
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


Αντικαθιστά το στοιχείο στη συγκεκριμένη θέση σε αυτή τη λίστα με το καθορισμένο στοιχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | \\{@inheritDoc\\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \\{@inheritDoc\\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο [CalendarCollection](../../com.aspose.tasks/calendarcollection).

**Returns:**
int - ο αριθμός των αντικειμένων που περιέχονται σε αυτό το αντικείμενο [CalendarCollection](../../com.aspose.tasks/calendarcollection).
### toList() {#toList--}
```
public final List<Calendar> toList()
```


Μετατρέπει το αντικείμενο CalendarCollection σε λίστα αντικειμένων [Calendar](../../com.aspose.tasks/calendar).

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - Λίστα αντικειμένων [Calendar](../../com.aspose.tasks/calendar).
