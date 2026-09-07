---
title: "Duration.Subtract"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Duration. Αφαιρεί τη συγκεκριμένη διάρκεια από αυτήν την παρουσία Duration."
type: docs
weight: 100
url: /el/net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

Αφαιρεί την καθορισμένη διάρκεια από αυτή την παρουσία διάρκειας.

```csharp
public Duration Subtract(Duration d)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| d | Duration | τη συγκεκριμένη παρουσία [`Duration`](../) για αφαίρεση από αυτήν την παρουσία. |

### Τιμή Επιστροφής

Νέο αντικείμενο διάρκειας που αντιπροσωπεύει την τιμή αυτής της παρουσίασης μείον τη συγκεκριμένη τιμή διάρκειας.

## Παραδείγματα

Δείχνει πώς να αλλάξετε τη διάρκεια των εργασιών.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// λάβετε μια εργασία
var task1 = project.RootTask.Children.GetById(1);

// ενημερώστε τη διάρκεια της εργασίας
var duration1 = task1.Get(Tsk.Duration);

// αφαιρέστε μία ημέρα από την εργασία 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// ορίστε μια νέα διάρκεια στην εργασία
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// λάβετε μια άλλη εργασία
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// αλλάξτε τη διάρκεια χρησιμοποιώντας τον πραγματικό τύπο μονάδας χρόνου
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// ορίστε μια νέα διάρκεια στην εργασία
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Δείτε επίσης

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

Αφαιρεί την καθορισμένη τιμή double από αυτή την παρουσία διάρκειας.

```csharp
public Duration Subtract(double val)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| val | Double | τη συγκεκριμένη τιμή Double για αφαίρεση από αυτήν την παρουσία. |

### Τιμή Επιστροφής

Νέο αντικείμενο διάρκειας που αντιπροσωπεύει την τιμή αυτής της παρουσίασης μείον τη συγκεκριμένη τιμή διάρκειας.

## Παραδείγματα

Δείχνει πώς να αλλάξετε τη διάρκεια των εργασιών.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// λάβετε μια εργασία
var task1 = project.RootTask.Children.GetById(1);

// ενημερώστε τη διάρκεια της εργασίας
var duration1 = task1.Get(Tsk.Duration);

// αφαιρέστε μία ημέρα από την εργασία 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// ορίστε μια νέα διάρκεια στην εργασία
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// λάβετε μια άλλη εργασία
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// αλλάξτε τη διάρκεια χρησιμοποιώντας τον πραγματικό τύπο μονάδας χρόνου
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// ορίστε μια νέα διάρκεια στην εργασία
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Δείτε επίσης

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


