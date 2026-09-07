---
title: "Calendar.GetFinishDateByStartAndWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Υπολογίζει την ημερομηνία όταν το καθορισμένο ποσό χρόνου εργασίας θα περάσει σύμφωνα με το ημερολόγιο."
type: docs
weight: 160
url: /el/net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

Υπολογίζει την ημερομηνία κατά την οποία θα περάσει η καθορισμένη ποσότητα χρόνου εργασίας σύμφωνα με το ημερολόγιο.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | DateTime | Ημερομηνία έναρξης. |
| εργασία | Διάρκεια | Διάρκεια εργασίας. |

### Τιμή Επιστροφής

Ημερομηνία λήξης.

## Παραδείγματα

Δείχνει πώς να υπολογίσετε μια ημερομηνία λήξης με βάση την ημερομηνία έναρξης και την εργασία χρησιμοποιώντας ένα στιγμιότυπο ημερολογίου.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// υπολογίστε την ημερομηνία λήξης χρησιμοποιώντας ένα τυπικό ημερολόγιο
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Δείτε επίσης

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

Υπολογίζει την ημερομηνία κατά την οποία θα περάσει η καθορισμένη ποσότητα χρόνου εργασίας σύμφωνα με το ημερολόγιο.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | DateTime | Ημερομηνία έναρξης. |
| εργασία | TimeSpan | Διάρκεια εργασίας. |

### Τιμή Επιστροφής

Ημερομηνία λήξης.

## Παραδείγματα

Δείχνει πώς να υπολογίσετε μια ημερομηνία λήξης με βάση την ημερομηνία έναρξης και την εργασία (ως χρονικό διάστημα) χρησιμοποιώντας ένα στιγμιότυπο ημερολογίου.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// υπολογίστε την ημερομηνία λήξης χρησιμοποιώντας ένα τυπικό ημερολόγιο
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


