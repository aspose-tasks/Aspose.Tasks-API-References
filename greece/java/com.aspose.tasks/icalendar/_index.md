---
title: "ICalendar"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά μια αφηρημένη αναπαράσταση ημερολογίου που μπορεί να χρησιμοποιηθεί για διάφορους υπολογισμούς ημερομηνιών και διάρκειας."
type: docs
weight: 376
url: /el/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

Αναπαριστά μια αφηρημένη αναπαράσταση ημερολογίου που μπορεί να χρησιμοποιηθεί για διάφορους υπολογισμούς ημερομηνιών και διάρκειας.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | Υπολογίζει την ημερομηνία κατά την οποία θα περάσει η καθορισμένη ποσότητα χρόνου εργασίας σύμφωνα με το ημερολόγιο. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | Υπολογίζει την ημερομηνία κατά την οποία θα περάσει η καθορισμένη ποσότητα χρόνου εργασίας σύμφωνα με το ημερολόγιο. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | Υπολογίζει την έναρξη της επόμενης εργάσιμης ημέρας για την καθορισμένη ημερομηνία. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | Υπολογίζει το τέλος της προηγούμενης εργάσιμης ημερομηνίας από την καθορισμένη ημερομηνία. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | Επιστρέφει την ημερομηνία έναρξης βάσει της καθορισμένης ημερομηνίας λήξης και της διάρκειας. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | Επιστρέφει την ημερομηνία έναρξης βάσει της καθορισμένης ημερομηνίας λήξης και της διάρκειας. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | Υπολογίζει την ημερομηνία και ώρα λήξης της εργασίας από την ημερομηνία έναρξής της, τα διαχωρισμένα τμήματα και τη διάρκεια εργασίας. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | Υπολογίζει την έναρξη του επόμενου εργάσιμου χρόνου ξεκινώντας από την καθορισμένη ημερομηνία και ώρα. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | Επιστρέφει την ποσότητα των εργάσιμων ωρών στην καθορισμένη ημερομηνία. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | Επιστρέφει το WorkUnit - Έναρξη, Λήξη και Διάρκεια των εργάσιμων ωρών για το καθορισμένο χρονικό διάστημα. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | Επιστρέφει την ποσότητα των εργάσιμων ωρών μεταξύ των καθορισμένων ημερομηνιών. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | Επιστρέφει το [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) των εργάσιμων χρόνων για την καθορισμένη ημερομηνία. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | Καθορίζει εάν η καθορισμένη ημέρα είναι εργάσιμη ημέρα σύμφωνα με το ημερολόγιο. |
| [isEmpty()](#isEmpty--) | Επιστρέφει εάν το ημερολόγιο δεν έχει ορισμένες εργάσιμες ώρες. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


Υπολογίζει την ημερομηνία κατά την οποία θα περάσει η καθορισμένη ποσότητα χρόνου εργασίας σύμφωνα με το ημερολόγιο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | java.util.Date | Ημερομηνία έναρξης. |
| work | [Duration](../../com.aspose.tasks/duration) | Διάρκεια εργασίας. |

**Returns:**
java.util.Date - Ημερομηνία λήξης.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


Υπολογίζει την ημερομηνία κατά την οποία θα περάσει η καθορισμένη ποσότητα χρόνου εργασίας σύμφωνα με το ημερολόγιο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | java.util.Date | Ημερομηνία έναρξης. |
| εργασία | double | Διάρκεια εργασίας. |

**Returns:**
java.util.Date - Ημερομηνία λήξης.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


Υπολογίζει την έναρξη της επόμενης εργάσιμης ημέρας για την καθορισμένη ημερομηνία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ημερομηνία | java.util.Date | Η ημερομηνία για την οποία θα ληφθεί η έναρξη της επόμενης εργάσιμης ημέρας. |

**Returns:**
java.util.Date - Έναρξη επόμενης εργάσιμης ημέρας System.DateTime.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


Υπολογίζει το τέλος της προηγούμενης εργάσιμης ημερομηνίας από την καθορισμένη ημερομηνία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ημερομηνία | java.util.Date | η ημερομηνία για τον υπολογισμό του τέλους της προηγούμενης εργάσιμης ημέρας. |

**Returns:**
java.util.Date - Το τέλος της προηγούμενης εργάσιμης ημέρας
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


Επιστρέφει την ημερομηνία έναρξης βάσει της καθορισμένης ημερομηνίας λήξης και της διάρκειας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| λήξη | java.util.Date | Η καθορισμένη ημερομηνία λήξης. |
| duration | [Duration](../../com.aspose.tasks/duration) | Η καθορισμένη διάρκεια. |

**Returns:**
java.util.Date - Υπολογισμένη ημερομηνία έναρξης.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


Επιστρέφει την ημερομηνία έναρξης βάσει της καθορισμένης ημερομηνίας λήξης και της διάρκειας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| λήξη | java.util.Date | Η καθορισμένη ημερομηνία λήξης. |
| διάρκεια | double | Η καθορισμένη διάρκεια. |

**Returns:**
java.util.Date - Υπολογισμένη ημερομηνία έναρξης.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


Υπολογίζει την ημερομηνία και ώρα λήξης της εργασίας από την ημερομηνία έναρξής της, τα διαχωρισμένα τμήματα και τη διάρκεια εργασίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Η εργασία για την οποία θα υπολογιστεί η ημερομηνία λήξης. |
|  | διάρκεια | double | Η διάρκεια προς υπολογισμό. |

Επιστρέφει DateTime.MinValue εάν η εργασία είναι σύνοψη, null ή η ημερομηνία έναρξής της δεν έχει οριστεί. |

**Returns:**
java.util.Date - Η ημερομηνία λήξης της εργασίας για την δεδομένη ημερομηνία έναρξης και διάρκεια.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


Υπολογίζει την έναρξη του επόμενου εργάσιμου χρόνου ξεκινώντας από την καθορισμένη ημερομηνία και ώρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ημερομηνία | java.util.Date | Η ημερομηνία και ώρα. |

**Returns:**
java.util.Date - Η πιο κοντινή έναρξη εργάσιμου χρόνου.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


Επιστρέφει την ποσότητα των εργάσιμων ωρών στην καθορισμένη ημερομηνία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dt | java.util.Date | Η ημερομηνία για την οποία θα ληφθούν οι εργάσιμες ώρες. |

**Returns:**
double - Εργάσιμες ώρες στην καθορισμένη ημερομηνία.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


Επιστρέφει το WorkUnit - Έναρξη, Λήξη και Διάρκεια των εργάσιμων ωρών για το καθορισμένο χρονικό διάστημα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | java.util.Date | Ημερομηνία έναρξης του διαστήματος. |
| λήξη | java.util.Date | Ημερομηνία λήξης του διαστήματος. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


Επιστρέφει την ποσότητα των εργάσιμων ωρών μεταξύ των καθορισμένων ημερομηνιών.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | java.util.Date | Ημερομηνία έναρξης του διαστήματος. |
| λήξη | java.util.Date | Ημερομηνία λήξης του διαστήματος. |

**Returns:**
double - Ποσό εργάσιμων ωρών σύμφωνα με το παράδειγμα ημερολογίου.
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


Επιστρέφει το [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) των εργάσιμων χρόνων για την καθορισμένη ημερομηνία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dt | java.util.Date | Η ημερομηνία για την οποία θα ληφθούν οι εργάσιμες ώρες. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


Καθορίζει εάν η καθορισμένη ημέρα είναι εργάσιμη ημέρα σύμφωνα με το ημερολόγιο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dt | java.util.Date | Η ημερομηνία για να ελεγχθεί αν η ημέρα είναι εργάσιμη. |

**Returns:**
boolean - Αληθές εάν η ημέρα είναι εργάσιμη.
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


Επιστρέφει εάν το ημερολόγιο δεν έχει ορισμένες εργάσιμες ώρες.

**Returns:**
boolean - Αληθές εάν το ημερολόγιο δεν έχει ορισμένες ώρες εργασίας.
