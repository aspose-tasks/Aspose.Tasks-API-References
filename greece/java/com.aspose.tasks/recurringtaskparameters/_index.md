---
title: "RecurringTaskParameters"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά το σύνολο των παραμέτρων που χρησιμοποιούνται για τη δημιουργία μιας επαναλαμβανόμενης εργασίας σε ένα έργο."
type: docs
weight: 245
url: /el/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

Αναπαριστά το σύνολο των παραμέτρων που χρησιμοποιούνται για τη δημιουργία μιας επαναλαμβανόμενης εργασίας σε ένα έργο.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDuration()](#getDuration--) | Λαμβάνει τη διάρκεια για μία εμφάνιση της επαναλαμβανόμενης εργασίας. |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | Λαμβάνει μια τιμή που υποδεικνύει αν θα προγραμματιστεί η επαναλαμβανόμενη εργασία ακόμη και αν δεν συμβαίνει όταν υπάρχουν διαθέσιμοι πόροι για να εργαστούν πάνω της. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Λαμβάνει το πρότυπο επανάληψης της επαναλαμβανόμενης εργασίας. |
| [getTaskName()](#getTaskName--) | Λαμβάνει το όνομα της επαναλαμβανόμενης εργασίας. |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | Ορίστε ένα ημερολόγιο για την επαναλαμβανόμενη εργασία. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Ορίζει τη διάρκεια για μία εμφάνιση της επαναλαμβανόμενης εργασίας. |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | Ορίζει μια τιμή που υποδεικνύει αν θα προγραμματιστεί η επαναλαμβανόμενη εργασία ακόμη και αν δεν συμβαίνει όταν υπάρχουν διαθέσιμοι πόροι για να εργαστούν πάνω της. |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | Ορίζει το πρότυπο επανάληψης της επαναλαμβανόμενης εργασίας. |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | Ορίζει το όνομα της επαναλαμβανόμενης εργασίας. |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters).

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Λαμβάνει τη διάρκεια για μία εμφάνιση της επαναλαμβανόμενης εργασίας.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


Λαμβάνει μια τιμή που υποδεικνύει αν θα προγραμματιστεί η επαναλαμβανόμενη εργασία ακόμη και αν δεν συμβαίνει όταν υπάρχουν διαθέσιμοι πόροι για να εργαστούν πάνω της.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν θα προγραμματιστεί η επαναλαμβανόμενη εργασία ακόμη και αν δεν μπορεί να εκτελεστεί όταν δεν υπάρχουν διαθέσιμοι πόροι για να εργαστούν σε αυτήν.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


Λαμβάνει το πρότυπο επανάληψης της επαναλαμβανόμενης εργασίας.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης `RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose/tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) enumeration.

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


Λαμβάνει το όνομα της επαναλαμβανόμενης εργασίας.

**Returns:**
java.lang.String - το όνομα της επαναλαμβανόμενης εργασίας.
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


Ορίστε ένα ημερολόγιο για την επαναλαμβανόμενη εργασία. Το ημερολόγιο επιλέγεται από τη συλλογή ημερολογίων του έργου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Το έργο με τη συλλογή ημερολογίων. |
| calendarName | java.lang.String | Το όνομα του ημερολογίου. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Ορίζει τη διάρκεια για μία εμφάνιση της επαναλαμβανόμενης εργασίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Το αντικείμενο της κλάσης `Duration`([getDuration()](../../com.aspose/tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose/tasks/recurringtaskparameters\#setDuration-Duration-)) class. |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν θα προγραμματιστεί η επαναλαμβανόμενη εργασία ακόμη και αν δεν συμβαίνει όταν υπάρχουν διαθέσιμοι πόροι για να εργαστούν πάνω της.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν θα προγραμματιστεί η επαναλαμβανόμενη εργασία ακόμη και αν δεν μπορεί να εκτελεστεί όταν δεν υπάρχουν διαθέσιμοι πόροι για να εργαστούν σε αυτήν. |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


Ορίζει το πρότυπο επανάληψης της επαναλαμβανόμενης εργασίας.

--------------------

Μπορεί να είναι μία από τις τιμές της απαρίθμησης `RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose/tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) enumeration.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | το πρότυπο επανάληψης της επαναλαμβανόμενης εργασίας. |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


Ορίζει το όνομα της επαναλαμβανόμενης εργασίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το όνομα της επαναλαμβανόμενης εργασίας. |

