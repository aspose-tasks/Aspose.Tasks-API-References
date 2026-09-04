---
title: "CalendarException"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά εξαιρετικές χρονικές περιόδους σε ένα ημερολόγιο."
type: docs
weight: 43
url: /el/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

Αναπαριστά εξαιρετικές χρονικές περιόδους σε ένα ημερολόγιο.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CalendarException()](#CalendarException--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [CalendarException](../../com.aspose.tasks/calendarexception). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | Επιστρέφει true εάν η καθορισμένη παρουσία της δομής java.util.Date είναι η ημέρα εξαίρεσης. |
| [delete()](#delete--) | Διαγράφει την παρουσία Exception από το γονικό αντικείμενο CalendarExceptionCollection του ημερολογίου. |
| [getDayWorking()](#getDayWorking--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι εργάσιμη. |
| [getDaysOfWeek()](#getDaysOfWeek--) | Αποκτά το DayTypeCollection για αυτό το αντικείμενο. |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | Αποκτά μια τιμή που υποδεικνύει εάν η περιοχή επανάληψης ορίζεται με την εισαγωγή αριθμού εμφανίσεων. |
| [getExceptionDates()](#getExceptionDates--) | Επιστρέφει ημερομηνίες στις οποίες η εξαίρεση ημερολογίου ισχύει. |
| [getFromDate()](#getFromDate--) | Αποκτά την έναρξη του χρόνου εξαίρεσης. |
| [getMonth()](#getMonth--) | Αποκτά το μήνα για τον οποίο έχει προγραμματιστεί η επανάληψη της εξαίρεσης. |
| [getMonthDay()](#getMonthDay--) | Αποκτά την ημέρα του μήνα στην οποία έχει προγραμματιστεί η επανάληψη της εξαίρεσης. |
| [getMonthItem()](#getMonthItem--) | Αποκτά το στοιχείο μήνα για τον οποίο έχει προγραμματιστεί η επανάληψη της εξαίρεσης. |
| [getMonthPosition()](#getMonthPosition--) | Αποκτά τη θέση ενός στοιχείου μήνα μέσα σε έναν μήνα. |
| [getName()](#getName--) | Αποκτά το όνομα της εξαίρεσης. |
| [getOccurrences()](#getOccurrences--) | Αποκτά τον αριθμό των εμφανίσεων για τις οποίες η εξαίρεση ημερολογίου είναι έγκυρη. |
| [getParentCalendar()](#getParentCalendar--) | Λαμβάνει το γονικό ημερολόγιο για αυτό το αντικείμενο. |
| [getPeriod()](#getPeriod--) | Αποκτά την περίοδο επανάληψης για την εξαίρεση. |
| [getToDate()](#getToDate--) | Αποκτά το τέλος του χρόνου εξαίρεσης. |
| [getType()](#getType--) | Αποκτά τον τύπο της εξαίρεσης. |
| [getWorkingTime()](#getWorkingTime--) | Επιστρέφει τον χρόνο εργασίας για μια εξαίρεση ημερολογίου. |
| [getWorkingTimes()](#getWorkingTimes--) | Αποκτά το αντικείμενο WorkingTimeCollection. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι εργάσιμη. |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν η περιοχή επανάληψης ορίζεται με την εισαγωγή αριθμού εμφανίσεων. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Ορίζει την έναρξη του χρόνου εξαίρεσης. |
| [setMonth(int value)](#setMonth-int-) | Ορίζει το μήνα για τον οποίο προγραμματίζεται η επανάληψη της εξαίρεσης. |
| [setMonthDay(int value)](#setMonthDay-int-) | Ορίζει την ημέρα του μήνα στην οποία προγραμματίζεται η επανάληψη της εξαίρεσης. |
| [setMonthItem(int value)](#setMonthItem-int-) | Ορίζει το στοιχείο του μήνα για τον οποίο προγραμματίζεται η επανάληψη της εξαίρεσης. |
| [setMonthPosition(int value)](#setMonthPosition-int-) | Ορίζει τη θέση ενός στοιχείου μήνα μέσα σε ένα μήνα. |
| [setName(String value)](#setName-java.lang.String-) | Ορίζει το όνομα της εξαίρεσης. |
| [setOccurrences(int value)](#setOccurrences-int-) | Ορίζει τον αριθμό των εμφανίσεων για τις οποίες η εξαίρεση του ημερολογίου είναι έγκυρη. |
| [setPeriod(int value)](#setPeriod-int-) | Ορίζει την περίοδο επανάληψης για την εξαίρεση. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Ορίζει το τέλος του χρόνου εξαίρεσης. |
| [setType(int value)](#setType-int-) | Ορίζει τον τύπο της εξαίρεσης. |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | Ορίζει το αντικείμενο WorkingTimeCollection. |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [CalendarException](../../com.aspose.tasks/calendarexception).

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


Επιστρέφει true εάν η καθορισμένη παρουσία της δομής java.util.Date είναι η ημέρα εξαίρεσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dt | java.util.Date | η καθορισμένη παρουσία της δομής java.util.Date. |

**Returns:**
boolean - Επιστρέφει true εάν η τιμή java.util.Date είναι η ημέρα της εξαίρεσης· διαφορετικά, false.
### delete() {#delete--}
```
public final void delete()
```


Διαγράφει την παρουσία Exception από το γονικό αντικείμενο CalendarExceptionCollection του ημερολογίου.

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι εργάσιμη.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι ενεργή.
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


Λαμβάνει το DayTypeCollection για αυτό το αντικείμενο. Οι ημέρες της εβδομάδας στις οποίες η εξαίρεση είναι έγκυρη.

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η περιοχή επανάληψης ορίζεται με την εισαγωγή αριθμού εμφανίσεων. False υποδεικνύει ότι η περιοχή επανάληψης ορίζεται με την εισαγωγή ημερομηνίας λήξης.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν η περιοχή επανάληψης ορίζεται με την εισαγωγή αριθμού εμφανίσεων.
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


Επιστρέφει ημερομηνίες στις οποίες η εξαίρεση ημερολογίου ισχύει.

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - ημερομηνίες στις οποίες η εξαίρεση του ημερολογίου ισχύει.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Αποκτά την έναρξη του χρόνου εξαίρεσης.

**Returns:**
java.util.Date - η έναρξη του χρόνου εξαίρεσης.
### getMonth() {#getMonth--}
```
public final int getMonth()
```


Αποκτά το μήνα για τον οποίο έχει προγραμματιστεί η επανάληψη της εξαίρεσης.

**Returns:**
int - ο μήνας για τον οποίο προγραμματίζεται η επανάληψη της εξαίρεσης.
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


Αποκτά την ημέρα του μήνα στην οποία έχει προγραμματιστεί η επανάληψη της εξαίρεσης.

**Returns:**
int - η ημέρα του μήνα στην οποία προγραμματίζεται η επανάληψη της εξαίρεσης.
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


Αποκτά το στοιχείο μήνα για τον οποίο έχει προγραμματιστεί η επανάληψη της εξαίρεσης.

**Returns:**
int - το στοιχείο του μήνα για τον οποίο προγραμματίζεται η επανάληψη της εξαίρεσης.
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


Αποκτά τη θέση ενός στοιχείου μήνα μέσα σε έναν μήνα.

**Returns:**
int - η θέση ενός στοιχείου μήνα μέσα σε ένα μήνα.
### getName() {#getName--}
```
public final String getName()
```


Αποκτά το όνομα της εξαίρεσης.

**Returns:**
java.lang.String - το όνομα της εξαίρεσης.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Αποκτά τον αριθμό των εμφανίσεων για τις οποίες η εξαίρεση ημερολογίου είναι έγκυρη.

**Returns:**
int - ο αριθμός των εμφανίσεων για τις οποίες η εξαίρεση του ημερολογίου είναι έγκυρη.
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


Λαμβάνει το γονικό ημερολόγιο για αυτό το αντικείμενο.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


Αποκτά την περίοδο επανάληψης για την εξαίρεση.

**Returns:**
int - η περίοδος επανάληψης για την εξαίρεση.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Αποκτά το τέλος του χρόνου εξαίρεσης.

**Returns:**
java.util.Date - το τέλος του χρόνου εξαίρεσης.
### getType() {#getType--}
```
public final int getType()
```


Αποκτά τον τύπο της εξαίρεσης.

**Returns:**
int - ο τύπος της εξαίρεσης.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Επιστρέφει τον χρόνο εργασίας για μια εξαίρεση ημερολογίου.

**Returns:**
double - Επιστρέφει τον χρόνο εργασίας για αυτήν την εξαίρεση ημερολογίου.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Αποκτά το αντικείμενο WorkingTimeCollection. Η συλλογή των χρόνων εργασίας που ορίζει τον χρόνο εργασίας στην ημέρα της εβδομάδας.

--------------------

Πρέπει να υπάρχει τουλάχιστον ένας χρόνος εργασίας, και δεν μπορεί να υπάρχουν περισσότεροι από πέντε.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι εργάσιμη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι ενεργή. |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν η περιοχή επανάληψης ορίζεται με την εισαγωγή αριθμού εμφανίσεων. Το False υποδεικνύει ότι η περιοχή επανάληψης ορίζεται με την εισαγωγή ημερομηνίας λήξης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν η περιοχή επανάληψης ορίζεται με την εισαγωγή αριθμού εμφανίσεων. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Ορίζει την έναρξη του χρόνου εξαίρεσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η αρχή του χρόνου εξαίρεσης. |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


Ορίζει το μήνα για τον οποίο προγραμματίζεται η επανάληψη της εξαίρεσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο μήνας για τον οποίο έχει προγραμματιστεί η επανάληψη της εξαίρεσης. |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


Ορίζει την ημέρα του μήνα στην οποία προγραμματίζεται η επανάληψη της εξαίρεσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | η ημέρα του μήνα στην οποία έχει προγραμματιστεί η επανάληψη της εξαίρεσης. |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


Ορίζει το στοιχείο του μήνα για τον οποίο προγραμματίζεται η επανάληψη της εξαίρεσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το στοιχείο μήνα για το οποίο έχει προγραμματιστεί η επανάληψη της εξαίρεσης. |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


Ορίζει τη θέση ενός στοιχείου μήνα μέσα σε ένα μήνα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | η θέση ενός στοιχείου μήνα μέσα σε έναν μήνα. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Ορίζει το όνομα της εξαίρεσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το όνομα της εξαίρεσης. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Ορίζει τον αριθμό των εμφανίσεων για τις οποίες η εξαίρεση του ημερολογίου είναι έγκυρη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο αριθμός των εμφανίσεων για τις οποίες η εξαίρεση ημερολογίου είναι έγκυρη. |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


Ορίζει την περίοδο επανάληψης για την εξαίρεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | η περίοδος επανάληψης για την εξαίρεση. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Ορίζει το τέλος του χρόνου εξαίρεσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | το τέλος του χρόνου εξαίρεσης. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Ορίζει τον τύπο της εξαίρεσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο τύπος της εξαίρεσης. |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


Ορίζει το αντικείμενο WorkingTimeCollection. Η συλλογή των χρόνων εργασίας που ορίζει τον χρόνο εργασίας στην ημέρα της εβδομάδας.

--------------------

Πρέπει να υπάρχει τουλάχιστον ένας χρόνος εργασίας, και δεν μπορεί να υπάρχουν περισσότεροι από πέντε.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | το αντικείμενο WorkingTimeCollection. |

