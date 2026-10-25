---
title: "Duration"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά τη διάρκεια σε ένα έργο."
type: docs
weight: 76
url: /el/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

Αναπαριστά τη διάρκεια σε ένα έργο.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Duration()](#Duration--) | Αρχικοποιεί ένα νέο στιγμιότυπο της δομής [Duration](../../com.aspose.tasks/duration) με μια καθορισμένη τιμή TimeSpan και TimeUnitType. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [Clone()](#Clone--) | Δημιουργεί και επιστρέφει ένα βαθύ αντίγραφο αυτού του παραδείγματος. |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | Δημιουργεί ένα βαθύ αντίγραφο της παρουσίασης σε άλλη παρουσίαση. |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | Προσθέτει την καθορισμένη διάρκεια σε αυτή τη διάρκεια. |
| [add(double val)](#add-double-) | Προσθέτει την καθορισμένη διπλή τιμή σε αυτή τη διάρκεια. |
| [clone()](#clone--) | \\{@inheritDoc\\} |
| [convert(byte timeUnitType)](#convert-byte-) | Μετατρέπει το αντικείμενο Duration σε άλλη διάρκεια με καθορισμένες μονάδες χρόνου. |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Επιστρέφει μια τιμή που υποδεικνύει αν η καθορισμένη παρουσία `obj1` είναι ίση με την καθορισμένη παρουσία `obj2`. |
| [equals(Object obj)](#equals-java.lang.Object-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [getTimeSpan()](#getTimeSpan--) | Λαμβάνει την παρουσία `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) αυτού του αντικειμένου Duration. |
| [getTimeUnit()](#getTimeUnit--) | Λαμβάνει τον τύπο μονάδας χρόνου για αυτό το αντικείμενο. |
| [hashCode()](#hashCode--) | Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο. |
| [isElapsed()](#isElapsed--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η μονάδα χρόνου είναι περασμένη. |
| [isEstimated()](#isEstimated--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η μονάδα χρόνου είναι εκτιμώμενη. |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο. |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | Μετατρέπει το καθορισμένο κείμενο στην παρουσία της δομής [Duration](../../com.aspose.tasks/duration). |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | Αναλύει τη συμβολοσειρά διάρκειας στη μορφή "PT--H--M--S--". |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | Αφαιρεί την καθορισμένη διάρκεια από αυτήν την παρουσία διάρκειας. |
| [subtract(double val)](#subtract-double-) | Αφαιρεί την καθορισμένη τιμή double από αυτήν την παρουσία διάρκειας. |
| [toDouble()](#toDouble--) | Μετατρέπει το αντικείμενο Duration σε τιμή `double`. |
| [toString()](#toString--) | Επιστρέφει μια αναπαράσταση κειμένου αυτής της παρουσίασης. |
### Duration() {#Duration--}
```
public Duration()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της δομής [Duration](../../com.aspose.tasks/duration) με μια καθορισμένη τιμή TimeSpan και TimeUnitType.

### Clone() {#Clone--}
```
public Duration Clone()
```


Δημιουργεί και επιστρέφει ένα βαθύ αντίγραφο αυτού του παραδείγματος.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


Δημιουργεί ένα βαθύ αντίγραφο της παρουσίασης σε άλλη παρουσίαση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | άλλη παρουσία. |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


Προσθέτει την καθορισμένη διάρκεια σε αυτή τη διάρκεια.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | η καθορισμένη [Duration](../../com.aspose.tasks/duration) για προσθήκη σε αυτήν την παρουσία. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


Προσθέτει την καθορισμένη διπλή τιμή σε αυτή τη διάρκεια.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| val | double | η καθορισμένη τιμή `double` για προσθήκη σε αυτήν την παρουσία. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### convert(byte timeUnitType) {#convert-byte-}
```
public final Duration convert(byte timeUnitType)
```


Μετατρέπει το αντικείμενο Duration σε άλλη διάρκεια με καθορισμένες μονάδες χρόνου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| timeUnitType | byte | ο καθορισμένος τύπος μονάδας χρόνου. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | Το αντικείμενο για σύγκριση με αυτήν την παρουσία. |

**Returns:**
boolean - Επιστρέφει **True** εάν η άλλη παρουσία Duration έχει τις ίδιες τιμές TimeSpan και TimeUnit με αυτήν την παρουσία· διαφορετικά, **false**.
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


Επιστρέφει μια τιμή που υποδεικνύει αν η καθορισμένη παρουσία `obj1` είναι ίση με την καθορισμένη παρουσία `obj2`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | το πρώτο αντικείμενο για σύγκριση. |
| obj2 | [Duration](../../com.aspose.tasks/duration) | το δεύτερο αντικείμενο για σύγκριση. |

**Returns:**
boolean - επιστρέφει true εάν η καθορισμένη παρουσία `obj1` είναι ίση με την καθορισμένη παρουσία `obj2`; διαφορετικά, false.
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
boolean - **True** εάν το καθορισμένο αντικείμενο είναι ένα Duration που έχει τις ίδιες τιμές TimeSpan και TimeUnit με αυτήν την παρουσία· διαφορετικά, **false**.
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


Λαμβάνει την παρουσία `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) αυτού του αντικειμένου Duration.

Τιμή: Η παρουσία TimeSpan αυτού του αντικειμένου Duration.

**Returns:**
double - παρουσία `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) αυτού του αντικειμένου Duration.
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


Λαμβάνει τον τύπο μονάδας χρόνου για αυτό το αντικείμενο.

Τιμή: Ο τύπος μονάδας χρόνου αυτής της παρουσίασης Duration.

**Returns:**
byte - τύπος μονάδας χρόνου για αυτό το αντικείμενο.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.

**Returns:**
int - επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτήν την παρουσία διάρκειας.
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η μονάδα χρόνου είναι περασμένη.

Τιμή: Η σημαία που καθορίζει εάν αυτή η παρουσία Duration είναι περασμένη.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν η μονάδα χρόνου είναι περασμένη.
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η μονάδα χρόνου είναι εκτιμώμενη.

Τιμή: Η σημαία που καθορίζει εάν αυτή η παρουσία Duration είναι εκτιμώμενη.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν η μονάδα χρόνου είναι εκτιμώμενη.
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | Η πρώτη διάρκεια. |
| b | [Duration](../../com.aspose.tasks/duration) | Η δεύτερη διάρκεια. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | Η πρώτη διάρκεια. |
| b | [Duration](../../com.aspose.tasks/duration) | Η δεύτερη διάρκεια. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


Μετατρέπει το καθορισμένο κείμενο στην παρουσία της δομής [Duration](../../com.aspose.tasks/duration).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | την καθορισμένη εμφάνιση της κλάσης [Project](../../com.aspose.tasks/project) για τη μετατροπή της διάρκειας. |
| τιμή | java.lang.String | τη καθορισμένη συμβολοσειρά για μετατροπή. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


Αναλύει τη συμβολοσειρά διάρκειας στη μορφή "PT--H--M--S--".

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | τη καθορισμένη συμβολοσειρά για ανάλυση. |

**Returns:**
double - επιστρέφει την αναλυμένη εμφάνιση του `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) struct.
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


Αφαιρεί την καθορισμένη διάρκεια από αυτήν την παρουσία διάρκειας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | την καθορισμένη εμφάνιση του [Duration](../../com.aspose.tasks/duration) για αφαίρεση από αυτήν την εμφάνιση. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


Αφαιρεί την καθορισμένη τιμή double από αυτήν την παρουσία διάρκειας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| val | double | την καθορισμένη τιμή `double` για αφαίρεση από αυτήν την εμφάνιση. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Μετατρέπει το αντικείμενο Duration σε τιμή `double`.

**Returns:**
double - Μετατρεπόμενη τιμή.
### toString() {#toString--}
```
public String toString()
```


Επιστρέφει μια αναπαράσταση κειμένου αυτής της παρουσίασης.

**Returns:**
java.lang.String - μια συμβολοσειρά αναπαράστασης αυτής της εμφάνισης.
