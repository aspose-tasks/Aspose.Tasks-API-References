---
title: "RecurringTaskInfo"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά τις λεπτομέρειες μιας επαναλαμβανόμενης εργασίας σε ένα έργο."
type: docs
weight: 244
url: /el/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

Αναπαριστά τις λεπτομέρειες μιας επαναλαμβανόμενης εργασίας σε ένα έργο.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | Λαμβάνει έναν αριθμό επαναλήψεων για το ημερήσιο μοτίβο επανάληψης. |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθούν εργάσιμες ημέρες για το ημερήσιο μοτίβο επανάληψης. |
| [getDuration()](#getDuration--) | Λαμβάνει τη διάρκεια για μία εμφάνιση της επαναλαμβανόμενης εργασίας. |
| [getEndDate()](#getEndDate--) | Λαμβάνει την ημερομηνία λήξης των εμφανίσεων. |
| [getMonthlyDay()](#getMonthlyDay--) | Λαμβάνει έναν αριθμό ημερών του μηνιαίου μοτίβου επανάληψης. |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | Λαμβάνει μια ημέρα του μηνιαίου μοτίβου επανάληψης όταν χρησιμοποιείται διατεταγμένη ημέρα. |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | Λαμβάνει έναν διατεταγμένο αριθμό του μηνιαίου μοτίβου επανάληψης. |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | Λαμβάνει έναν αριθμό επαναλήψεων για το μηνιαίο μοτίβο επανάληψης όταν χρησιμοποιείται διατεταγμένη ημέρα. |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | Λαμβάνει έναν αριθμό επαναλήψεων για το μηνιαίο μοτίβο επανάληψης. |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί διατεταγμένη ημέρα για το μηνιαίο μοτίβο επανάληψης. |
| [getOccurrences()](#getOccurrences--) | Λαμβάνει έναν αριθμό εμφανίσεων της επαναλαμβανόμενης εργασίας. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Λαμβάνει ένα μοτίβο επανάληψης της επαναλαμβανόμενης εργασίας. |
| [getStartDate()](#getStartDate--) | Λαμβάνει την ημερομηνία έναρξης των εμφανίσεων. |
| [getTask()](#getTask--) | Λαμβάνει την γονική εργασία αυτής της παρουσίας της κλάσης [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo). |
| [getUseEndDate()](#getUseEndDate--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί η ημερομηνία λήξης ή ένας αριθμός εμφανίσεων για την επαναλαμβανόμενη εργασία. |
| [getWeeklyDays()](#getWeeklyDays--) | Λαμβάνει μια συλλογή ημερών που χρησιμοποιούνται στο εβδομαδιαίο μοτίβο επανάληψης. |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | Λαμβάνει έναν αριθμό επαναλήψεων για το εβδομαδιαίο μοτίβο επανάληψης. |
| [getYearlyDate()](#getYearlyDate--) | Λαμβάνει μια ημερομηνία για το ετήσιο μοτίβο επανάληψης. |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | Λαμβάνει μια ημέρα της εβδομάδας του ετήσιου προτύπου επανάληψης όταν χρησιμοποιείται η διατεταγμένη ημέρα. |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | Λαμβάνει ένα μήνα του ετήσιου προτύπου επανάληψης όταν χρησιμοποιείται η διατεταγμένη ημέρα. |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | Λαμβάνει έναν διατεταγμένο αριθμό του ετήσιου προτύπου επανάληψης. |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί η διατεταγμένη ημέρα για το ετήσιο πρότυπο επανάληψης. |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | Ορίζει έναν αριθμό επαναλήψεων για το καθημερινό πρότυπο επανάληψης. |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθούν εργάσιμες ημέρες για το καθημερινό πρότυπο επανάληψης. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Ορίζει τη διάρκεια για μία εμφάνιση της επαναλαμβανόμενης εργασίας. |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Ορίζει την ημερομηνία λήξης των εμφανίσεων. |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | Ορίζει έναν αριθμό ημέρας του μηνιαίου προτύπου επανάληψης. |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | Ορίζει μια ημέρα του μηνιαίου προτύπου επανάληψης όταν χρησιμοποιείται η διατεταγμένη ημέρα. |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | Ορίζει έναν διατεταγμένο αριθμό του μηνιαίου προτύπου επανάληψης. |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | Ορίζει έναν αριθμό επαναλήψεων για το μηνιαίο πρότυπο επανάληψης όταν χρησιμοποιείται η διατεταγμένη ημέρα. |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | Ορίζει έναν αριθμό επαναλήψεων για το μηνιαίο πρότυπο επανάληψης. |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί η διατεταγμένη ημέρα για το μηνιαίο πρότυπο επανάληψης. |
| [setOccurrences(int value)](#setOccurrences-int-) | Ορίζει έναν αριθμό εμφανίσεων της επαναλαμβανόμενης εργασίας. |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | Ορίζει ένα πρότυπο επανάληψης της επαναλαμβανόμενης εργασίας. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Ορίζει την ημερομηνία έναρξης των εμφανίσεων. |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί η ημερομηνία λήξης ή ένας αριθμός εμφανίσεων για την επαναλαμβανόμενη εργασία. |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | Ορίζει μια συλλογή ημερών που χρησιμοποιούνται στο εβδομαδιαίο πρότυπο επανάληψης. |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | Ορίζει έναν αριθμό επαναλήψεων για το εβδομαδιαίο πρότυπο επανάληψης. |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | Ορίζει μια ημερομηνία για το ετήσιο πρότυπο επανάληψης. |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | Ορίζει μια ημέρα της εβδομάδας του ετήσιου προτύπου επανάληψης όταν χρησιμοποιείται η διατεταγμένη ημέρα. |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | Ορίζει ένα μήνα του ετήσιου προτύπου επανάληψης όταν χρησιμοποιείται η διατεταγμένη ημέρα. |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | Ορίζει έναν διατεταγμένο αριθμό του ετήσιου προτύπου επανάληψης. |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί η διατεταγμένη ημέρα για το ετήσιο πρότυπο επανάληψης. |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


Λαμβάνει έναν αριθμό επαναλήψεων για το ημερήσιο μοτίβο επανάληψης.

**Returns:**
int - ένας αριθμός επαναλήψεων για το ημερήσιο μοτίβο επανάληψης.
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθούν εργάσιμες ημέρες για το ημερήσιο μοτίβο επανάληψης.

**Returns:**
boolean - τιμή που υποδεικνύει εάν θα χρησιμοποιηθούν εργάσιμες ημέρες για το ημερήσιο μοτίβο επανάληψης.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Λαμβάνει τη διάρκεια για μία εμφάνιση της επαναλαμβανόμενης εργασίας.

--------------------

η παρουσία της κλάσης `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)).

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Λαμβάνει την ημερομηνία λήξης των εμφανίσεων.

**Returns:**
java.util.Date - η ημερομηνία λήξης των εμφανίσεων.
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


Λαμβάνει έναν αριθμό ημερών του μηνιαίου μοτίβου επανάληψης.

**Returns:**
int - ένας αριθμός ημέρας του μηνιαίου μοτίβου επανάληψης.
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


Λαμβάνει μια ημέρα του μηνιαίου μοτίβου επανάληψης όταν χρησιμοποιείται διατεταγμένη ημέρα.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Returns:**
int - μια ημέρα του μηνιαίου μοτίβου επανάληψης όταν χρησιμοποιείται διατεταγμένη ημέρα.
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


Λαμβάνει έναν διατεταγμένο αριθμό του μηνιαίου μοτίβου επανάληψης.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Returns:**
int - ένας διατεταγμένος αριθμός του μηνιαίου μοτίβου επανάληψης.
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


Λαμβάνει έναν αριθμό επαναλήψεων για το μηνιαίο μοτίβο επανάληψης όταν χρησιμοποιείται διατεταγμένη ημέρα.

**Returns:**
int - ένας αριθμός επαναλήψεων για το μηνιαίο μοτίβο επανάληψης όταν χρησιμοποιείται διατεταγμένη ημέρα.
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


Λαμβάνει έναν αριθμό επαναλήψεων για το μηνιαίο μοτίβο επανάληψης.

**Returns:**
int - ένας αριθμός επαναλήψεων για το μηνιαίο μοτίβο επανάληψης.
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί διατεταγμένη ημέρα για το μηνιαίο μοτίβο επανάληψης.

**Returns:**
boolean - τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί διατεταγμένη ημέρα για το μηνιαίο μοτίβο επανάληψης.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Λαμβάνει έναν αριθμό εμφανίσεων της επαναλαμβανόμενης εργασίας.

**Returns:**
int - ένας αριθμός εμφανίσεων της επαναλαμβανόμενης εργασίας.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


Λαμβάνει ένα μοτίβο επανάληψης της επαναλαμβανόμενης εργασίας.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)).

**Returns:**
int - ένα μοτίβο επανάληψης της επαναλαμβανόμενης εργασίας.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Λαμβάνει την ημερομηνία έναρξης των εμφανίσεων.

**Returns:**
java.util.Date - η ημερομηνία έναρξης των εμφανίσεων.
### getTask() {#getTask--}
```
public final Task getTask()
```


Λαμβάνει την γονική εργασία αυτής της παρουσίας της κλάσης [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo).

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί η ημερομηνία λήξης ή ένας αριθμός εμφανίσεων για την επαναλαμβανόμενη εργασία.

**Returns:**
boolean - τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί η ημερομηνία λήξης ή ένας αριθμός εμφανίσεων για την επαναλαμβανόμενη εργασία.
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


Λαμβάνει μια συλλογή ημερών που χρησιμοποιούνται στο εβδομαδιαίο μοτίβο επανάληψης.

--------------------

**Returns:**
int - μια συλλογή ημερών που χρησιμοποιούνται στο εβδομαδιαίο μοτίβο επανάληψης.
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


Λαμβάνει έναν αριθμό επαναλήψεων για το εβδομαδιαίο μοτίβο επανάληψης.

**Returns:**
int - ένας αριθμός επαναλήψεων για το εβδομαδιαίο μοτίβο επανάληψης.
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


Λαμβάνει μια ημερομηνία για το ετήσιο μοτίβο επανάληψης.

**Returns:**
java.util.Date - μια ημερομηνία για το ετήσιο μοτίβο επανάληψης.
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


Λαμβάνει μια ημέρα της εβδομάδας του ετήσιου προτύπου επανάληψης όταν χρησιμοποιείται η διατεταγμένη ημέρα.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Returns:**
int - μια ημέρα της εβδομάδας του ετήσιου μοτίβου επανάληψης όταν χρησιμοποιείται διατεταγμένη ημέρα.
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


Λαμβάνει ένα μήνα του ετήσιου προτύπου επανάληψης όταν χρησιμοποιείται η διατεταγμένη ημέρα.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης [Month](../../com.aspose.tasks/month).

**Returns:**
int - ένας μήνας του ετήσιου μοτίβου επανάληψης όταν χρησιμοποιείται διατεταγμένη ημέρα.
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


Λαμβάνει έναν διατεταγμένο αριθμό του ετήσιου προτύπου επανάληψης.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Returns:**
int - ένας διατεταγμένος αριθμός του ετήσιου μοτίβου επανάληψης.
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί η διατεταγμένη ημέρα για το ετήσιο πρότυπο επανάληψης.

**Returns:**
boolean - τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί διατεταγμένη ημέρα για το ετήσιο μοτίβο επανάληψης.
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


Ορίζει έναν αριθμό επαναλήψεων για το καθημερινό πρότυπο επανάληψης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | αριθμός επαναλήψεων για το ημερήσιο πρότυπο επανάληψης. |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθούν εργάσιμες ημέρες για το καθημερινό πρότυπο επανάληψης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | τιμή που υποδεικνύει εάν θα χρησιμοποιηθούν εργάσιμες ημέρες για το ημερήσιο πρότυπο επανάληψης. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Ορίζει τη διάρκεια για μία εμφάνιση της επαναλαμβανόμενης εργασίας.

--------------------

η παρουσία της κλάσης `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | η διάρκεια για μία εμφάνιση της επαναλαμβανόμενης εργασίας. |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Ορίζει την ημερομηνία λήξης των εμφανίσεων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η ημερομηνία λήξης των εμφανίσεων. |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


Ορίζει έναν αριθμό ημέρας του μηνιαίου προτύπου επανάληψης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | αριθμός ημέρας του μηνιαίου προτύπου επανάληψης. |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


Ορίζει μια ημέρα του μηνιαίου προτύπου επανάληψης όταν χρησιμοποιείται η διατεταγμένη ημέρα.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια ημέρα του μηνιαίου προτύπου επανάληψης όταν χρησιμοποιείται διατεταγμένη ημέρα. |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


Ορίζει έναν διατεταγμένο αριθμό του μηνιαίου προτύπου επανάληψης.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένας διατεταγμένος αριθμός του μηνιαίου προτύπου επανάληψης. |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


Ορίζει έναν αριθμό επαναλήψεων για το μηνιαίο πρότυπο επανάληψης όταν χρησιμοποιείται η διατεταγμένη ημέρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | αριθμός επαναλήψεων για το μηνιαίο πρότυπο επανάληψης όταν χρησιμοποιείται διατεταγμένη ημέρα. |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


Ορίζει έναν αριθμό επαναλήψεων για το μηνιαίο πρότυπο επανάληψης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | αριθμός επαναλήψεων για το μηνιαίο πρότυπο επανάληψης. |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί η διατεταγμένη ημέρα για το μηνιαίο πρότυπο επανάληψης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί διατεταγμένη ημέρα για το μηνιαίο πρότυπο επανάληψης. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Ορίζει έναν αριθμό εμφανίσεων της επαναλαμβανόμενης εργασίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | αριθμός εμφανίσεων της επαναλαμβανόμενης εργασίας. |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


Ορίζει ένα πρότυπο επανάληψης της επαναλαμβανόμενης εργασίας.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένα πρότυπο επανάληψης της επαναλαμβανόμενης εργασίας. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Ορίζει την ημερομηνία έναρξης των εμφανίσεων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η ημερομηνία έναρξης των εμφανίσεων. |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί η ημερομηνία λήξης ή ένας αριθμός εμφανίσεων για την επαναλαμβανόμενη εργασία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί η ημερομηνία λήξης ή αριθμός εμφανίσεων για την επαναλαμβανόμενη εργασία. |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


Ορίζει μια συλλογή ημερών που χρησιμοποιούνται στο εβδομαδιαίο πρότυπο επανάληψης.

--------------------

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια συλλογή ημερών που χρησιμοποιούνται στο εβδομαδιαίο πρότυπο επανάληψης. |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


Ορίζει έναν αριθμό επαναλήψεων για το εβδομαδιαίο πρότυπο επανάληψης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | αριθμός επαναλήψεων για το εβδομαδιαίο πρότυπο επανάληψης. |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


Ορίζει μια ημερομηνία για το ετήσιο πρότυπο επανάληψης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η ημερομηνία για το ετήσιο πρότυπο επανάληψης. |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


Ορίζει μια ημέρα της εβδομάδας του ετήσιου προτύπου επανάληψης όταν χρησιμοποιείται η διατεταγμένη ημέρα.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια ημέρα της εβδομάδας του ετήσιου προτύπου επανάληψης όταν χρησιμοποιείται διατεταγμένη ημέρα. |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


Ορίζει ένα μήνα του ετήσιου προτύπου επανάληψης όταν χρησιμοποιείται η διατεταγμένη ημέρα.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης [Month](../../com.aspose.tasks/month).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένας μήνας του ετήσιου προτύπου επανάληψης όταν χρησιμοποιείται διατεταγμένη ημέρα. |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


Ορίζει έναν διατεταγμένο αριθμό του ετήσιου προτύπου επανάληψης.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένας διατεταγμένος αριθμός του ετήσιου προτύπου επανάληψης. |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί η διατεταγμένη ημέρα για το ετήσιο πρότυπο επανάληψης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί διατεταγμένη ημέρα για το ετήσιο πρότυπο επανάληψης. |

