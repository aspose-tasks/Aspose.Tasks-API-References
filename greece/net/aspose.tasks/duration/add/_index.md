---
title: "Duration.Add"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Duration. Προσθέτει την καθορισμένη διάρκεια σε αυτή τη διάρκεια."
type: docs
weight: 60
url: /el/net/aspose.tasks/duration/add/
---
## Add(Duration) {#add}

Προσθέτει την καθορισμένη διάρκεια σε αυτή τη διάρκεια.

```csharp
public Duration Add(Duration d)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| d | Duration | την καθορισμένη [`Duration`](../) για προσθήκη σε αυτό το παράδειγμα. |

### Τιμή Επιστροφής

Νέο αντικείμενο διάρκειας που αντιπροσωπεύει την τιμή αυτού του αντικειμένου συν την καθορισμένη τιμή διάρκειας.

## Παραδείγματα

Δείχνει πώς να ενημερώσετε μια διάρκεια εργασιών.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// λάβετε μια εργασία
var task1 = project.RootTask.Children.GetById(1);

// ενημερώστε τη διάρκεια της εργασίας
var duration1 = task1.Get(Tsk.Duration);

// προσθέστε μία ημέρα στην εργασία 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// ορίστε μια νέα διάρκεια στην εργασία
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// λάβετε μια άλλη εργασία
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// αλλάξτε τη διάρκεια χρησιμοποιώντας τον πραγματικό τύπο μονάδας χρόνου
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// ορίστε μια νέα διάρκεια στην εργασία
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### Δείτε επίσης

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Add(double) {#add_1}

Προσθέτει την καθορισμένη τιμή double σε αυτή τη διάρκεια.

```csharp
public Duration Add(double val)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| val | Double | η καθορισμένη τιμή Double που θα προστεθεί σε αυτό το αντικείμενο. |

### Τιμή Επιστροφής

Νέο αντικείμενο διάρκειας που αντιπροσωπεύει την τιμή αυτού του αντικειμένου συν την καθορισμένη τιμή διάρκειας.

## Παραδείγματα

Δείχνει πώς να ενημερώσετε μια διάρκεια εργασιών.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// λάβετε μια εργασία
var task1 = project.RootTask.Children.GetById(1);

// ενημερώστε τη διάρκεια της εργασίας
var duration1 = task1.Get(Tsk.Duration);

// προσθέστε μία ημέρα στην εργασία 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// ορίστε μια νέα διάρκεια στην εργασία
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// λάβετε μια άλλη εργασία
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// αλλάξτε τη διάρκεια χρησιμοποιώντας τον πραγματικό τύπο μονάδας χρόνου
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// ορίστε μια νέα διάρκεια στην εργασία
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### Δείτε επίσης

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


