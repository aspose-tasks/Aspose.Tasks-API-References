---
title: "Δομή Duration"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Duration δομή. Αντιπροσωπεύει τη διάρκεια σε ένα έργο."
type: docs
weight: 470
url: /el/net/aspose.tasks/duration/
---
## Duration structure

Αναπαριστά τη διάρκεια σε ένα έργο.

```csharp
public struct Duration : IEquatable<Duration>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει αν η μονάδα χρόνου έχει παρέλθει. Η σημαία που καθορίζει αν αυτή η παρουσία Duration έχει παρέλθει. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει αν η μονάδα χρόνου είναι εκτιμώμενη. Η σημαία που καθορίζει αν αυτή η παρουσία Duration είναι εκτιμώμενη. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | Λαμβάνει την παρουσία [`TimeSpan`](./timespan/) αυτού του αντικειμένου Duration. Η παρουσία TimeSpan αυτού του αντικειμένου Duration. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | Λαμβάνει τον τύπο μονάδας χρόνου για αυτό το αντικείμενο. Ο τύπος μονάδας χρόνου της παρουσίας Duration. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | Μετατρέπει το καθορισμένο κείμενο στην παρουσία της δομής `Duration`. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | Προσθέτει την καθορισμένη τιμή double σε αυτή τη διάρκεια. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | Προσθέτει την καθορισμένη διάρκεια σε αυτή τη διάρκεια. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Μετατρέπει το αντικείμενο Duration σε άλλη διάρκεια με καθορισμένες μονάδες χρόνου. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | Αφαιρεί την καθορισμένη τιμή double από αυτή την παρουσία διάρκειας. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | Αφαιρεί την καθορισμένη διάρκεια από αυτή την παρουσία διάρκειας. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Μετατρέπει το αντικείμενο Duration σε τιμή Double. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | Επιστρέφει μια αναπαράσταση string αυτής της παρουσίας. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | Αναλύει το κείμενο διάρκειας στη μορφή "PT--H--M--S--". |
| [operator ==](../../aspose.tasks/duration/op_equality/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


