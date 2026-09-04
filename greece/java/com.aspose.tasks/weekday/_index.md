---
title: "Ημέρα Εβδομάδας"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά μια ημέρα της εβδομάδας που είτε ορίζει κανονικές ημέρες της εβδομάδας είτε ημέρες εξαίρεσης σε ένα ημερολόγιο."
type: docs
weight: 352
url: /el/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

Αναπαριστά μια ημέρα της εβδομάδας που είτε ορίζει κανονικές ημέρες της εβδομάδας είτε ημέρες εξαίρεσης σε ένα ημερολόγιο.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [WeekDay](../../com.aspose.tasks/weekday) με τον καθορισμένο τύπο ημέρας. |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [WeekDay](../../com.aspose.tasks/weekday) με τον καθορισμένο τύπο ημέρας και λίστα περιόδων εργασίας. |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [WeekDay](../../com.aspose.tasks/weekday) με τον καθορισμένο τύπο ημέρας και περιόδους εργασίας. |
| [WeekDay()](#WeekDay--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [WeekDay](../../com.aspose.tasks/weekday). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | Μετατρέπει το [DayOfWeek](../../com.aspose.tasks/dayofweek) του .Net σε `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)). |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | Δημιουργεί προεπιλεγμένη εργάσιμη ημέρα. |
| [deepClone()](#deepClone--) | Επιστρέφει ένα βαθύ αντίγραφο της ημέρας της εβδομάδας. |
| [equals(Object obj)](#equals-java.lang.Object-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [getDayType()](#getDayType--) | Λαμβάνει τον τύπο μιας ημέρας. |
| [getDayWorking()](#getDayWorking--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι εργάσιμη. |
| [getFromDate()](#getFromDate--) | Λαμβάνει την αρχή μιας εξαιρετικής χρονικής περιόδου. |
| [getToDate()](#getToDate--) | Λαμβάνει το τέλος μιας εξαιρετικής χρονικής περιόδου. |
| [getWorkingTime()](#getWorkingTime--) | Επιστρέφει τον χρόνο εργασίας για μια ημέρα της εβδομάδας. |
| [getWorkingTimes()](#getWorkingTimes--) | Λαμβάνει το WorkingTimeCollection για αυτήν την παρουσία του WeekDay. |
| [hashCode()](#hashCode--) | Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης [WeekDay](../../com.aspose.tasks/weekday). |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι εργάσιμη. |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | Ορίζει προεπιλεγμένες χρονικές περιόδους για την καθορισμένη ημέρα της εβδομάδας. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Ορίζει την αρχή μιας εξαιρετικής χρονικής περιόδου. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Ορίζει το τέλος μιας εξαιρετικής χρονικής περιόδου. |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [WeekDay](../../com.aspose.tasks/weekday) με τον καθορισμένο τύπο ημέρας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dayType | int | Ο καθορισμένος τύπος ημέρας. |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [WeekDay](../../com.aspose.tasks/weekday) με τον καθορισμένο τύπο ημέρας και λίστα περιόδων εργασίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dayType | int | Ο καθορισμένος τύπος ημέρας. |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | Λίστα χρονικών περιόδων εργασίας. |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [WeekDay](../../com.aspose.tasks/weekday) με τον καθορισμένο τύπο ημέρας και περιόδους εργασίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dayType | int | Ο καθορισμένος τύπος ημέρας. |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | Πίνακας χρονικών περιόδων εργασίας. |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [WeekDay](../../com.aspose.tasks/weekday).

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


Μετατρέπει το [DayOfWeek](../../com.aspose.tasks/dayofweek) του .Net σε `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dw | int | Η ημέρα της εβδομάδας από την οποία θα μετατραπεί. |

**Returns:**
int - Ένας τύπος ημέρας μετά τη μετατροπή.
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


Δημιουργεί προεπιλεγμένη εργάσιμη ημέρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dayType | int | Ο τύπος ημέρας από τον οποίο θα δημιουργηθεί η προεπιλεγμένη εργάσιμη ημέρα. |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


Επιστρέφει ένα βαθύ αντίγραφο της ημέρας της εβδομάδας.

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
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
boolean - **True** εάν το καθορισμένο αντικείμενο είναι ένα WeekDay που έχει τις ίδιες τιμές FromDate, ToDate και WorkingTimes με αυτήν την περίπτωση· διαφορετικά, **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


Λαμβάνει τον τύπο μιας ημέρας.

**Returns:**
int - ο τύπος μιας ημέρας.
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι εργάσιμη.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι ενεργή.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Λαμβάνει την αρχή μιας εξαιρετικής χρονικής περιόδου.

**Returns:**
java.util.Date - η αρχή μιας χρονικής εξαίρεσης.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Λαμβάνει το τέλος μιας εξαιρετικής χρονικής περιόδου.

**Returns:**
java.util.Date - το τέλος μιας χρονικής εξαίρεσης.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Επιστρέφει τον χρόνο εργασίας για μια ημέρα της εβδομάδας.

**Returns:**
double - Χρόνος εργασίας.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Λαμβάνει το WorkingTimeCollection για αυτήν την περίπτωση WeekDay. Η συλλογή των χρόνων εργασίας που ορίζουν τον χρόνο που εργάζεται την ημέρα της εβδομάδας.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης [WeekDay](../../com.aspose.tasks/weekday).

**Returns:**
int - επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι εργάσιμη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι ενεργή. |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


Ορίζει προεπιλεγμένες χρονικές περιόδους για την καθορισμένη ημέρα της εβδομάδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | Η ημέρα της εβδομάδας στην οποία θα οριστεί η προεπιλεγμένη εργάσιμη ημέρα. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Ορίζει την αρχή μιας εξαιρετικής χρονικής περιόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η αρχή μιας χρονικής εξαίρεσης. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Ορίζει το τέλος μιας εξαιρετικής χρονικής περιόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | το τέλος μιας χρονικής εξαίρεσης. |

