---
title: "WorkingTime"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά έναν χρόνο εργασίας κατά τη διάρκεια μιας ημέρας της εβδομάδας."
type: docs
weight: 365
url: /el/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

Αναπαριστά έναν χρόνο εργασίας κατά τη διάρκεια μιας ημέρας της εβδομάδας.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [WorkingTime](../../com.aspose.tasks/workingtime) με ένα διάστημα με τις καθορισμένες ώρες έναρξης και λήξης. |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [WorkingTime](../../com.aspose.tasks/workingtime) με ένα στοιχείο διαστήματος με τις καθορισμένες ώρες έναρξης και λήξης. |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [WorkingTime](../../com.aspose.tasks/workingtime) με ένα στοιχείο διαστήματος με τις καθορισμένες ώρες έναρξης και λήξης. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Ελέγχει ότι τα αντικείμενα είναι ίσα. |
| [getFrom()](#getFrom--) | Λαμβάνει την αρχή ενός χρόνου εργασίας. |
| [getTo()](#getTo--) | Λαμβάνει το τέλος ενός χρόνου εργασίας. |
| [hashCode()](#hashCode--) | Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης [WorkingTime](../../com.aspose.tasks/workingtime). |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [WorkingTime](../../com.aspose.tasks/workingtime) με ένα διάστημα με τις καθορισμένες ώρες έναρξης και λήξης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fromTime | java.util.Date | ώρα έναρξης διαστήματος |
| toTime | java.util.Date | ώρα λήξης διαστήματος |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [WorkingTime](../../com.aspose.tasks/workingtime) με ένα στοιχείο διαστήματος με τις καθορισμένες ώρες έναρξης και λήξης.

--------------------

&gt; ```
&gt; Η υπερφόρτωση του κατασκευαστή WorkingTime μπορεί να χρησιμοποιηθεί για την αρχικοποίηση της έναρξης και λήξης του διαστήματος χρησιμοποιώντας TimeSpans:
&gt; ``````

 [C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | double | Interval's start time represented by double struct. |
| toTime | double | Interval's end time represented by double struct. |

### WorkingTime(int fromHours, int toHours) {#WorkingTime-int-int-}
```
public WorkingTime(int fromHours, int toHours)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times.

--------------------

&gt; ```
&gt; The overload of WorkingTime ctor can be used to initialize interval's start and end using whole hours:
&gt; ``````

 [C#]
 var wt = new WorkingTime(9, 13);
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fromHours | int | Η ώρα έναρξης του διαστήματος αντιπροσωπεύεται από ολόκληρο αριθμό ωρών (0-24). |
| toHours | int | Η ώρα λήξης του διαστήματος αντιπροσωπεύεται από ολόκληρο αριθμό ωρών (0-24). |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Ελέγχει ότι τα αντικείμενα είναι ίσα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | java.lang.Object | Δεύτερο αντικείμενο για σύγκριση. |

**Returns:**
boolean - Αληθές εάν τα αντικείμενα είναι ίσα, ψευδές διαφορετικά.
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


Λαμβάνει την αρχή ενός χρόνου εργασίας.

**Returns:**
java.util.Date - η αρχή ενός χρόνου εργασίας.
### getTo() {#getTo--}
```
public final Date getTo()
```


Λαμβάνει το τέλος ενός χρόνου εργασίας.

**Returns:**
java.util.Date - το τέλος ενός χρόνου εργασίας.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης [WorkingTime](../../com.aspose.tasks/workingtime).

**Returns:**
int - επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.
