---
title: "Calendar.GetTaskFinishDateFromDuration"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Υπολογίζει την ημερομηνία και ώρα λήξης της εργασίας από τα τμήματα της ημερομηνίας έναρξης και τη διάρκεια εργασίας"
type: docs
weight: 210
url: /el/net/aspose.tasks/calendar/gettaskfinishdatefromduration/
---
## Calendar.GetTaskFinishDateFromDuration method

Υπολογίζει την ημερομηνία και ώρα λήξης της εργασίας από την ημερομηνία έναρξής της, τα διαχωρισμένα μέρη και τη διάρκεια εργασίας.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| εργασία | Εργασία | Η εργασία για την οποία θα υπολογιστεί η ημερομηνία λήξης. |
| διάρκεια | TimeSpan | Η διάρκεια προς υπολογισμό. |

### Τιμή Επιστροφής

Η ημερομηνία λήξης της εργασίας για την δεδομένη ημερομηνία έναρξης και διάρκεια.

## Παρατηρήσεις

Επιστρέφει DateTime.MinValue εάν η εργασία είναι σύνοψη, null ή η ημερομηνία έναρξής της δεν έχει οριστεί.

## Παραδείγματα

Δείχνει πώς να υπολογίσετε την ημερομηνία λήξης μιας εργασίας με προσαρμοσμένη διάρκεια.

```csharp
var project = new Project(DataDir + "SplitTaskFinishDate.mpp");

// Βρείτε μια διαχωρισμένη εργασία
var task = project.RootTask.Children.GetByUid(4);

// Βρείτε το ημερολόγιο του έργου
var calendar = project.Get(Prj.Calendar);

// Υπολογίστε την ημερομηνία λήξης της εργασίας με διαφορετικές διάρκειες
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 8 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(8, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 16 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(16, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 24 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(24, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 28 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(28, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 32 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(32, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 46 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(46, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 61 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(61, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 75 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(75, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 80 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(80, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 120 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(120, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 150 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(150, 0, 0)));
```

### Δείτε επίσης

* class [Task](../../task/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


